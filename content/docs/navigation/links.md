---
weight: 5
bookFlatSection: true
title: "友链"
---

<h1><b><i class="fa fa-hand-peace-o"></i> 友情链接</b></h1>

{{< hint info >}} 
**<i class="fa fa-exclamation-circle"></i>** 页面旨在聚集志同道合的小伙伴，欢迎与我取得[**联系**](mailto:leejiawang@live.com)。
{{< /hint >}}

站名 |  站点描述
:-- | :-- 
[程序羊 CodeSheep](https://www.codesheep.cn/) | 分享 务实、能看懂、读者可复现 的原创文章
[心谭博客](https://xin-tan.com/) | 专注于前端方向与可视化领域的博客
[利隐客 leeyiner](https://leeyiner.github.io/) | Find what you want

<div id="gitalk-container"></div>
<link rel="stylesheet" href="https://unpkg.com/gitalk/dist/gitalk.css">
<script src="https://unpkg.com/gitalk/dist/gitalk.min.js"></script>
<script>
  const gitalk = new Gitalk({
    clientID: '04cf552a019468513eda',
    clientSecret: '98ecb20a4ff40c3d1f6a6388c303fb443509bacf',
    repo: 'leejiawang.github.io',
    owner: 'leejiawang',
    admin: ['leejiawang'],
    id: location.blog.eyecus.links, // Ensure uniqueness and length less than 50
    distractionFreeMode: false // Facebook-like distraction free mode
  });
  (function() {
    if (["localhost", "127.0.0.1"].indexOf(window.location.hostname) != -1) {
      document.getElementById('gitalk-container').innerHTML = 'Gitalk comments not available by default when the website is previewed locally.';
      return;
    }
    gitalk.render('gitalk-container');
  })();
</script>

<div>&nbsp&nbsp&nbsp&nbsp</div>

<div align="center">  
<h3>👨🏻‍💻 期待您的加入...</h3>
</div>

