杏盛娱乐主管【Q-——333307——】杏盛娱乐主管【 辋芷《888yx●vip》 】
杏盛娱乐主管【Q-——333307——】杏盛娱乐主管【 辋芷《888yx●vip》 】

 从零搭建个人博客：GitHub Pages + Hexo 完整教程（2025版）

> 想拥有一个免费、稳定、可自定义的个人博客？这篇教程带你用 GitHub Pages 和 Hexo 从零开始，三十分钟上线。

---

 为什么选择 GitHub Pages + Hexo？

在众多博客方案中，这套组合优势明显：

- 完全免费：托管在 GitHub 上，无需服务器费用
- 极速访问：GitHub CDN 全球加速，国内访问速度尚可
- 版本管理：文章自动备份，写坏了随时回滚
- 生态丰富：Hexo 有 600+ 主题和插件，扩展方便

 环境准备

开始前，请确保本地已安装：

1. Node.js（v16 及以上）— [官网下载](https://nodejs.org/)
2. Git — [官网下载](https://git-scm.com/)
3. GitHub 账号 — 没有先注册一个

```bash
 验证安装
node -v
git --version
```

 三步搭建流程

 第一步：安装 Hexo 并初始化项目

```bash
 全局安装 hexo-cli
npm install -g hexo-cli

 初始化博客目录
hexo init my-blog
cd my-blog

 安装依赖
npm install
```

 第二步：本地预览

```bash
 启动本地服务
hexo server
```

访问 `http://localhost:4000`，看到默认博客即成功。

 第三步：部署到 GitHub Pages

创建仓库：在 GitHub 新建仓库，命名为 `你的用户名.github.io`

修改配置（`_config.yml` 文件）：

```yaml
deploy:
  type: git
  repo: https://github.com/你的用户名/你的用户名.github.io.git
  branch: main
```

部署命令：

```bash
npm install hexo-deployer-git --save
hexo clean && hexo generate && hexo deploy
```

等待 2-3 分钟，访问 `https://你的用户名.github.io` 即可看到你的博客。

---

 个性化技巧

- 更换主题：搜索 `hexo theme`，在[主题市场](https://hexo.io/themes/)挑选，下载后修改 `_config.yml` 中的 `theme` 字段
- 绑定域名：在仓库 Settings → Pages 中配置自定义域名，并在域名服务商添加 CNAME 记录

---

 常见问题排查

| 问题 | 解决方案 |
|------|----------|
| `hexo deploy` 报错 | 先执行 `npm install hexo-deployer-git --save` |
| 图片不显示 | 使用绝对路径 `/img/xxx.jpg`，存放于 `source/img/` |
| 访问 404 | 确认仓库名是否与用户名完全一致 |

---

 写在最后

搭建博客只是开始，坚持写作才是核心。建议每周更新一篇，哪怕只是技术笔记。

如果你在搭建过程中遇到任何问题，欢迎在评论区留言。

觉得有用的话，点个 ⭐ 或转发给需要的朋友，让更多人学会！

相关推荐：

https://github.com/brownbarbara40/yzuprm/blob/main/2027%E5%AE%98%E6%96%B9%E8%AE%B2%E8%A7%A3%EF%BC%9A%E6%9D%8F%E7%9B%9B%E5%A8%B1%E4%B9%90%E5%BC%80%E6%88%B7_%E9%93%BA%E8%A1%99%E6%99%AF%E7%9F%AB%E7%A6%84sxers.md

<img src="https://i.postimg.cc/bvDn3j3m/xingsheng-00014.png" />

相关推荐：

https://github.com/brownbarbara40/yzuprm/commit/0f71190f8b10a798677ca439f7555349e91c8c59

<img src="https://i.postimg.cc/SNkWq3xn/xingsheng-00009.png" />
相关推荐：

https://github.com/bakerangela2326/pvryuo/blob/main/2027%E5%AE%98%E7%BD%91%E6%95%99%E7%A8%8B%EF%BC%9A%E6%9D%8F%E7%9B%9B%E5%A8%B1%E4%B9%90%E6%B5%8B%E9%80%9F_%E6%95%85%E6%B5%A6%E6%B7%B3%E8%B9%AC%E8%A2%84fyyeu.md

<img src="https://i.postimg.cc/7hyS5Q1V/xingsheng-00005.png" />
相关推荐：

https://github.com/bakerangela2326/pvryuo/commit/f227b372e6a40d324572c3dbf3f9c9cce4d901f6

<img src="https://i.postimg.cc/7ZL0JzzN/xingsheng-00011.png" />

资讯来源：新华网、人民网、央视新闻、中新网、凤凰网、澎湃新闻、界面新闻、新浪新闻、搜狐网、财新网、观察者网、第一财经等主流平台，以独树一帜的观察视角与扎实的深度报道能力，在资讯领域收获广泛关注。
