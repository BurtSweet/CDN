<p id="hitokoto">:D 获取中...</p>
<script src="https://cdn.jsdelivr.net/npm/bluebird@3/js/browser/bluebird.min.js"></script＞
<script src="https://cdn.jsdelivr.net/npm/whatwg-fetch@2.0.3/fetch.min.js"></script＞
<!--End-->
<script＞
  fetch('https://v1.hitokoto.cn/?c=a&c=b&c=c&c=d&c=e&c=h&c=i&c=k')
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
</script＞
<div align="center"><iframe width=100% height=50% src="https://ip.skk.moe/simple" frameborder="1px"></iframe></div>
