<!-- ⛅ 实时天气（基于和风天气） -->
<div id="weather" style="margin-bottom: 10px;">
  <iframe width="100%" height="60" frameborder="0" scrolling="no"
    src="https://widget.qweather.net/simple/static/index.html?location=101190101&lang=zh&unit=c&theme=light">
  </iframe>
</div>

<!-- 🕒 实时时钟 -->
<div id="clock" style="font-size: 18px; font-weight: bold; margin-bottom: 10px;"></div>
<script>
  function updateClock() {
    const now = new Date();
    const timeStr = now.toLocaleTimeString('zh-CN', { hour12: false });
    const dateStr = now.toLocaleDateString('zh-CN');
    document.getElementById('clock').innerText = `🕒 当前时间：${dateStr} ${timeStr}`;
  }
  setInterval(updateClock, 1000);
  updateClock();
</script>

<!-- 👁️ 访客统计（基于 Busuanzi） -->
<div id="busuanzi_container_site_pv" style="font-size: 14px; color: #666;">
  👁️ 本站总访问量：<span id="busuanzi_value_site_pv"></span> 次
</div>
<script async src="https://busuanzi.icodeq.com/busuanzi/2.3/busuanzi.pure.mini.js"></script>
