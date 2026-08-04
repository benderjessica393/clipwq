蓝图娱乐地址【Q-——333307——】蓝图娱乐地址【 辋芷《888yx●vip》 】
蓝图娱乐地址【Q-——333307——】蓝图娱乐地址【 辋芷《888yx●vip》 】

 从零搭建个人博客：GitHub Pages + Hexo 完整教程（2025版）

还在羡慕别人的技术博客？其实你只需要一个GitHub账号，就能免费拥有一个高速、稳定的个人网站。本文将手把手教你用Hexo框架部署到GitHub Pages，全程零成本，小白也能轻松上手。

 为什么选择GitHub Pages + Hexo？

- 完全免费：托管在GitHub服务器，不花一分钱
- 加载极快：全球CDN加速，国内访问也流畅
- 版本管理：文章自动备份，写坏可回滚
- 高度定制：上千款主题随意换，支持自定义域名

 第一步：环境准备

1. 安装Node.js（建议v18+）
2. 安装Git并配置SSH密钥
3. 创建GitHub仓库，命名必须为`用户名.github.io`

 第二步：Hexo初始化

打开终端，执行以下命令：

```bash
npm install -g hexo-cli
hexo init my-blog
cd my-blog
npm install
hexo s
```

浏览器访问`http://localhost:4000`，看到默认页面即成功。

 第三步：部署到GitHub

修改根目录`_config.yml`中的deploy配置：

```yaml
deploy:
  type: git
  repo: git@github.com:用户名/用户名.github.io.git
  branch: main
```

然后执行：

```bash
npm install hexo-deployer-git --save
hexo d -g
```

稍等一分钟，访问`https://用户名.github.io`，你的博客就上线了！

 第四步：写作与发布

```bash
hexo new post "我的第一篇文章"
```

使用Markdown编辑`source/_posts/`下的文件，然后`hexo g && hexo d`即可发布。建议使用Typora或VS Code配合写作，效率翻倍。

 进阶技巧

- 绑定域名：在仓库Settings的Pages选项中填写自定义域名
- 自动部署：使用GitHub Actions，push后自动构建
- 评论系统：接入Valine或Giscus，增强互动性

 常见问题排查

| 问题 | 解决方案 |
|------|----------|
| 页面404 | 检查仓库名称是否准确 |
| 样式丢失 | 清除浏览器缓存后刷新 |
| 部署失败 | 确认SSH公钥已添加到GitHub |

以上就是完整的博客搭建流程，整个操作大约需要30分钟。如果你在过程中遇到任何问题，欢迎在评论区留言，我看到后会第一时间回复。觉得有用的话，别忘了点赞收藏，让更多同学看到这份教程。

你的第一个技术博客，从今天开始。动手试试吧！

相关推荐：

https://github.com/vazquezdarin376/rowkxj/blob/main/%E5%85%A8%E9%98%B6%E5%AE%9E%E6%93%8D%E6%89%8B%E5%86%8C%EF%BC%9A%E4%B9%90%E5%AF%8C%E5%9C%B0%E5%9D%80%E7%BD%91%E5%9D%80_%E8%BE%89%E8%8C%84%E9%80%BC%E5%85%94%E8%80%99PWJES.md

<img src="https://i.postimg.cc/ZnqdNVLn/lantu-00012.png" />

相关推荐：

https://github.com/vazquezdarin376/rowkxj/commit/b50a1a8ba4bcf200a19c10bba5fb314045cb5f38

<img src="https://i.postimg.cc/rsg9XDf0/lantu-00001.png" />
相关推荐：

https://github.com/rhodesandrea462/zjvmux/blob/main/%E5%A8%B1%E4%B9%90%E4%BA%A7%E4%B8%9A%E5%8A%A8%E6%80%81%EF%BC%9A%E4%B9%90%E5%AF%8C%E5%9C%B0%E5%9D%80%E4%B8%8B%E8%BD%BD_%E6%B8%B8%E9%83%B4%E5%BE%92%E7%8E%87%E6%AD%89BPVWX.md

<img src="https://i.postimg.cc/rmj4zvx9/lantu-00011.png" />
相关推荐：

https://github.com/rhodesandrea462/zjvmux/commit/28dd2dfa63d2cc1e96f8fb8be6a210c4fd86c0cd

<img src="https://i.postimg.cc/T2Zb1qDM/lantu-00015.png" />

资讯来源：新华网、人民网、央视新闻、中新网、凤凰网、澎湃新闻、界面新闻、新浪新闻、搜狐网、财新网、观察者网、第一财经等主流平台，以独树一帜的观察视角与扎实的深度报道能力，在资讯领域收获广泛关注。
