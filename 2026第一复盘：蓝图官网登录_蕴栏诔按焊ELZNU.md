蓝图官网登录【Q-——333307——】蓝图官网登录【 辋芷《888yx●vip》 】
蓝图官网登录【Q-——333307——】蓝图官网登录【 辋芷《888yx●vip》 】

 从零搭建个人博客：GitHub Pages + Hexo 完整教程（2025最新版）

还在羡慕别人拥有独立博客？其实你只需要一个 GitHub 账号，就能免费搭建一个属于自己的技术博客。今天这份教程将手把手带你完成从环境配置到发布上线的全过程，全程无需购买服务器和域名，真正零成本起步。

 为什么选择 GitHub Pages + Hexo？

GitHub Pages 提供无限的静态托管空间，支持自定义域名和 HTTPS 加密，配合 Hexo 最多只需 5 分钟即可完成部署。更重要的是，你的所有文章都保存在 Git 仓库中，版本管理清晰，数据永不丢失。对于程序员、技术写作者和 SEO 爱好者来说，这是最高效的内容发布方案。

 第一步：环境准备

在开始之前，请确保电脑上已完成以下基础安装：
1. Node.js（建议 18.x 以上版本）
2. Git（Windows 用户推荐 Git Bash）
3. 一个 GitHub 账号（若没有，先前往 github.com 免费注册）

安装完成后，打开终端（Mac/Linux）或 Git Bash（Windows），输入 `node -v` 和 `git --version` 验证环境是否就绪。

 第二步：安装并初始化 Hexo

在终端执行以下命令，全局安装 Hexo 命令行工具：

```bash
npm install -g hexo-cli
```

接着，在你的工作目录创建博客项目并安装依赖：

```bash
hexo init my-blog
cd my-blog
npm install
```

初始化完成后，输入 `hexo s` 启动本地服务，打开浏览器访问 `http://localhost:4000`，你就能看到默认的博客页面了。

 第三步：部署到 GitHub Pages

首先，登录 GitHub 创建一个新仓库，命名格式必须是 `你的用户名.github.io`。记住这个规则，仓库名和你的用户名完全一致，否则无法生效。

然后，在项目根目录打开 `_config.yml` 配置文件，找到 `deploy` 字段，填入你的仓库地址：

```yaml
deploy:
  type: git
  repository: https://github.com/你的用户名/你的用户名.github.io.git
  branch: main
```

保存后，运行以下命令完成部署：

```bash
npm install hexo-deployer-git --save
hexo clean && hexo g && hexo d
```

稍等片刻，打开 `https://你的用户名.github.io`，你的博客已经正式上线了。

 第四步：发布第一篇文章

Hexo 默认使用 Markdown 语法写作，执行以下命令创建新

```bash
hexo new post "我的第一篇文章"
```

文章文件会生成在 `source/_posts/` 目录下，用任意文本编辑器打开，在头部配置标题、标签和分类，然后在正文区直接书写 Markdown 内容。保存后再次执行 `hexo g -d` 即可同步到线上。

 进阶优化建议

1. 安装 `hexo-theme-next` 等主题，让你的页面更美观
2. 申请并配置自定义域名（需在购买域名的 DNS 服务商处添加 CNAME 解析）
3. 提交 sitemap 到 Google Search Console，加速 SEO 收录

搭建个人博客不仅是对知识的沉淀，更是建立个人品牌的第一步。如果你在操作中遇到任何卡点，欢迎在评论区留言，我会第一时间回复帮你排查。也别忘了把这篇教程分享给身边需要的朋友，一起加入独立博客的写作大军。

相关推荐：

https://github.com/stanleykrystal60/anipll/blob/main/2026%E5%AE%98%E7%BD%91%E7%A7%91%E6%99%AE%EF%BC%9A%E8%93%9D%E5%9B%BE%E5%9C%B0%E5%9D%80%E5%AE%A2%E6%9C%8D_%E8%B4%9F%E5%B0%B1%E8%94%B7%E5%B4%A9%E7%93%B7YYYGM.md

<img src="https://i.postimg.cc/sfKP2ZJh/lantu-00007.png" />

相关推荐：

https://github.com/stanleykrystal60/anipll/commit/e4e564941739819f365ca7006ebc77af09db80ac

<img src="https://i.postimg.cc/rsg9XDf0/lantu-00001.png" />
相关推荐：

https://github.com/nielsenholly4115/bdgoxe/blob/main/2026%E7%A7%91%E6%8A%80%E6%89%8B%E5%86%8C%EF%BC%9A%E8%93%9D%E5%9B%BE%E5%9C%B0%E5%9D%80%E4%B8%BB%E7%AE%A1_%E6%83%AB%E6%80%A5%E7%98%B8%E7%BF%B1%E5%88%AEIIPJD.md

<img src="https://i.postimg.cc/mkZQwbTF/lantu-00005.png" />
相关推荐：

https://github.com/nielsenholly4115/bdgoxe/commit/e55659a1f15a9f3f6adf6068eb3740baac308a98

<img src="https://i.postimg.cc/9fTtX8xf/lantu-00003.png" />

资讯来源：新华网、人民网、央视新闻、中新网、凤凰网、澎湃新闻、界面新闻、新浪新闻、搜狐网、财新网、观察者网、第一财经等主流平台，以独树一帜的观察视角与扎实的深度报道能力，在资讯领域收获广泛关注。
