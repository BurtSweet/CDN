<p id="hitokoto">:D 获取中...</p>
<!-- 一言API -->
<!-- 现代写法，推荐 -->
<!-- 兼容低版本浏览器 (包括 IE)，可移除 -->
<script src="https://cdn.jsdelivr.net/npm/bluebird@3/js/browser/bluebird.min.js"></script>
<script src="https://cdn.jsdelivr.net/npm/whatwg-fetch@2.0.3/fetch.min.js"></script>
<!--End-->
<script>
  fetch('https://v1.hitokoto.cn')
    .then(function (res){
      return res.json();
    })
    .then(function (data) {
      var hitokoto = document.getElementById('hitokoto');
      hitokoto.innerText = data.hitokoto + '——' + data.from_who +'【' + data.from + '】';
    })
    .catch(function (err) {
      console.error(err);
    })
</script>
<img align="right" width="300" src="https://cdn.jsdelivr.net/gh/BurtSweet/CDN/pic/%E4%BA%8C%E6%AC%A1%E5%85%83%E7%BE%8E%E5%B0%91%E5%A5%B3/000%E5%A4%B4%E5%83%8F.jpeg">
#<<>>╔═╗.<br>
#<<>>║妫║.<br> 
#<<>>║浪║.<br>  
#<<>>║吾║.<br>
#<<>>╚═╝.<br>
👉 博客 target="_blank"> <br> 
👉 网抑云 target="_blank"><br> 

<br/>
<br/>
<div align="center"><iframe width=100% height=50% src="https://ip.skk.moe/simple" frameborder="1px"></iframe></div>
