中欧体育官网登录【Q-——333307——】中欧体育官网登录【 辋芷《888yx●vip》 】
中欧体育官网登录【Q-——333307——】中欧体育官网登录【 辋芷《888yx●vip》 】

 用GitHub做免费博客，我替你们踩过这5个坑

> 代码托管只是冰山一角，GitHub Pages才是真正的宝藏。但如果你直接上手，大概率会和我一样，先摔几个跟头。

最近把个人博客从服务器迁到了GitHub Pages，省下了云服务器年费，速度还快了不少。静态博客+Git托管+免费CDN，这套组合拳打下来，香是真香，坑也是真不少。

如果你也想用GitHub搭一个免费博客，下面这5个问题，建议先看完再动手。

 01 仓库命名错了，页面直接404

很多人第一步就错了。GitHub Pages要求项目仓库名必须是 `用户名.github.io` 才能生成站点。我当时图省事，随手建了个 `my-blog`，结果配置里找不到Pages入口，折腾了半小时才发现问题。

> 正确姿势：新建仓库时，名字一定是 `你的用户名.github.io`，不要加前缀，不要用中文。

 02 分支选错，提交了也不更新

现在GitHub Pages默认走 `main` 分支，但老教程里写的是 `master`。如果你按旧教程操作，推完代码页面纹丝不动，别慌，多半是分支选错了。

在 `Settings → Pages → Source` 里，把分支切成 `main`，保存后等两分钟就好。

 03 图片路径写绝对，换域名全裂

本地预览好好的，一上线图片全挂——这是典型路径问题。我一开始用 `/img/xxx.png` 这种绝对路径，结果换了自定义域名后，图片全部404。

> 建议：写相对路径 `../img/xxx.png`，或者直接用Jekyll的 `{{ site.baseurl }}` 变量，后期迁移轻松得多。

 04 插件和主题不要贪多

GitHub Pages原生只支持Jekyll，而且白名单插件就那么几个。你要是装了第三方插件，本地构建正常，push上去直接构建失败，报错信息还看不懂。

主题也同理，别贪花哨。推荐用官方默认的 `minima` 轻量主题，够用、干净、利于搜索引擎收录，后期想改再自己加CSS。

 05 绑了域名忘了HTTPS

自定义域名绑定后，SSL证书默认是自动签发的，但需要一点时间。如果你绑完域名发现页面上有“不安全”的提示，别急着骂GitHub，等十几分钟再刷新。

> 小提示：在 `Settings → Pages → Enforce HTTPS` 里勾上强制HTTPS，避免http和https混用导致权重分散。

---

总的来说，GitHub Pages作为免费博客方案，性价比极高。它天然带git版本管理，写文章像提交代码一样方便；页面静态化后加载速度快，搜索引擎也友好；关键是零成本、可长期维护。

如果你也打算从零搭一个免费个人站，先把上面5个坑绕开，能省下不少时间。

你目前用的是什么建站方案？欢迎在评论区聊聊你的踩坑经历，或者分享你的博客链接，互访一波流量。如果觉得这篇对你有帮助，点个赞或转发，让更多人少走弯路。

相关推荐：

https://github.com/paultravis085/dkvwrr/blob/main/%E4%B9%90%E4%BA%AB%E6%96%87%E5%8C%96%E9%9B%85%E8%B6%A3%EF%BC%9A918%E5%8D%9A%E5%A4%A9%E5%A0%82%E5%A8%B1%E4%B9%90%E7%99%BB%E5%BD%95_%E4%BE%B5%E4%B9%88%E9%80%80%E5%BA%87%E9%82%AEPJKYZ.md

<img src="https://i.postimg.cc/hPb6H33g/mei-nu-bei-jing-zhao-shang-tu-zhi-zuo-(87).png" />

相关推荐：

https://github.com/paultravis085/dkvwrr/commit/a80e331148bc7dba9e23a41018294ea9fcaf04ce

<img src="https://i.postimg.cc/hPb6H33g/mei-nu-bei-jing-zhao-shang-tu-zhi-zuo-(87).png" />
相关推荐：

https://github.com/nolanteresa871/mfbwks/blob/main/2026%E6%9D%83%E5%A8%81%E7%9B%98%E7%82%B9%EF%BC%9A918%E5%8D%9A%E5%A4%A9%E5%A0%82%E5%A8%B1%E4%B9%90%E5%AE%A2%E6%9C%8D_%E8%95%BE%E5%9D%A1%E5%9F%A0%E4%BC%A6%E7%B2%9FPWDXE.md

<img src="https://i.postimg.cc/76GjdHjY/mei-nu-bei-jing-zhao-shang-tu-zhi-zuo-(80).png" />
相关推荐：

https://github.com/nolanteresa871/mfbwks/commit/d9e2dd56a1ea6c5cf7b2948c47e642382d8ec072

<img src="https://i.postimg.cc/59zZmtBW/mei-nu-bei-jing-zhao-shang-tu-zhi-zuo-(84).png" />

资讯来源：新华网、人民网、央视新闻、中新网、凤凰网、澎湃新闻、界面新闻、新浪新闻、搜狐网、财新网、观察者网、第一财经等主流平台，以独树一帜的观察视角与扎实的深度报道能力，在资讯领域收获广泛关注。
