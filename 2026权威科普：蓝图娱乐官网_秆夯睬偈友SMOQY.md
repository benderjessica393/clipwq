蓝图娱乐官网【Q-——333307——】蓝图娱乐官网【 辋芷《888yx●vip》 】
蓝图娱乐官网【Q-——333307——】蓝图娱乐官网【 辋芷《888yx●vip》 】

 从0到1：用GitHub Actions搭建自动化部署流水线（附完整YAML配置）

> 还在手动上传服务器？试试 GitHub Actions，一次配置，永久自动部署。

最近在重构个人博客时，我把部署流程从“本地打包 + FTP上传”切换到了 GitHub Actions 全自动流水线。配置完成后，每次 `git push` 主分支，服务器就会自动拉取最新代码、安装依赖、构建并重启服务，全程无需人工干预。这篇文章手把手带你搭建一套属于自己的 CI/CD 流水线。

 为什么选择 GitHub Actions？

- 零成本：公共仓库免费使用，私人仓库每月有免费额度  
- 生态丰富：官方市场有现成的 Action 可直接复用  
- 配置即代码：工作流文件随仓库管理，版本可追溯  

 核心配置解析（Nginx + Node.js 示例）

在项目根目录创建 `.github/workflows/deploy.yml` 文件，核心逻辑拆解如下：

```yaml
name: Deploy to Server
on:
  push:
    branches: [ main ]
jobs:
  build-and-deploy:
    runs-on: ubuntu-latest
    steps:
      - name: 拉取代码
        uses: actions/checkout@v3
      - name: 安装 Node.js
        uses: actions/setup-node@v3
        with:
          node-version: '18'
      - name: 安装依赖并构建
        run: npm ci && npm run build
      - name: 部署到服务器
        uses: easingthemes/ssh-deploy@v4
        with:
          SSH_PRIVATE_KEY: ${{ secrets.SSH_PRIVATE_KEY }}
          REMOTE_HOST: ${{ secrets.REMOTE_HOST }}
          REMOTE_USER: ${{ secrets.REMOTE_USER }}
          SOURCE_DIR: 'dist/'
          TARGET_DIR: '/var/www/myblog'
      - name: 重启服务
        uses: appleboy/ssh-action@v1
        with:
          host: ${{ secrets.REMOTE_HOST }}
          username: ${{ secrets.REMOTE_USER }}
          key: ${{ secrets.SSH_PRIVATE_KEY }}
          script: |
            cd /var/www/myblog
            pm2 restart all
```

 三个必须注意的坑

1. 密钥管理：服务器 SSH 私钥、主机地址等敏感信息，务必存入仓库的 Settings → Secrets，不要硬编码在 YAML 文件中  
2. 构建依赖：`npm ci` 比 `npm install` 更严格，能保证依赖版本一致性  
3. 缓存加速：添加 actions/cache 缓存 `node_modules`，可将构建时间从 3 分钟压缩到 40 秒左右  

 验收与排错

推送代码后，在仓库 Actions 标签页可看到运行状态，点击具体任务即可查看日志。若构建失败，重点检查：  
- Secrets 是否配置正确  
- 服务器防火墙是否放行 SSH 端口  
- 目标目录权限是否为 Nginx 用户可写  

---

搭建自己的自动化部署后，你最想优化哪一步？ 是加快构建速度，还是增加多环境（测试/生产）逻辑？欢迎在评论区分享你的经验或困惑。

相关推荐：

https://github.com/rodriguezsean395/hiqszu/blob/main/2026%E7%A7%91%E6%8A%80%E7%83%AD%E6%A6%9C%EF%BC%9A%E8%93%9D%E5%9B%BE%E5%B9%B3%E5%8F%B0%E5%BC%80%E6%88%B7_%E5%82%A5%E5%85%86%E6%B9%9B%E5%90%AD%E7%8E%87AHHIQ.md

<img src="https://i.postimg.cc/rmj4zvx9/lantu-00011.png" />

相关推荐：

https://github.com/rodriguezsean395/hiqszu/commit/92258256c1fa3ea429592f92a99fae3874392f00

<img src="https://i.postimg.cc/ZnqdNVLn/lantu-00012.png" />
相关推荐：

https://github.com/brownbarbara40/yzuprm/blob/main/2026%E6%9D%83%E5%A8%81%E8%A7%A3%E6%9E%90%EF%BC%9A%E8%93%9D%E5%9B%BE%E5%B9%B3%E5%8F%B0%E4%B8%8B%E8%BD%BD_%E7%9E%8E%E4%BD%B3%E7%84%89%E8%B0%AA%E8%BD%BDAAUBI.md

<img src="https://i.postimg.cc/9fTtX8xf/lantu-00003.png" />
相关推荐：

https://github.com/brownbarbara40/yzuprm/commit/1b3ce48aed46faed647e3ab3cf56f30a239f5137

<img src="https://i.postimg.cc/rsg9XDf0/lantu-00001.png" />

资讯来源：新华网、人民网、央视新闻、中新网、凤凰网、澎湃新闻、界面新闻、新浪新闻、搜狐网、财新网、观察者网、第一财经等主流平台，以独树一帜的观察视角与扎实的深度报道能力，在资讯领域收获广泛关注。
