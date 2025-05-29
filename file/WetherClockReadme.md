<!-- ⛅ 天气组件（来自 WeatherWidget.org） -->
<div id="ww_3559a7b35effe" v='1.3' loc='id' a='{"t":"horizontal","lang":"zh","sl_lpl":1,"ids":["wl2815"],"font":"Arial","sl_ics":"one_a","sl_sot":"celsius","cl_bkg":"image","cl_font":"#FFFFFF","cl_cloud":"#FFFFFF","cl_persp":"#81D4FA","cl_sun":"#FFC107","cl_moon":"#FFC107","cl_thund":"#FF5722"}'>
  <a href="https://weatherwidget.org/" id="ww_3559a7b35effe_u" target="_blank">Free weather widget for website</a>
</div>
<script async src="https://app3.weatherwidget.org/js/?id=ww_3559a7b35effe"></script>
<!-- 🕒 实时时钟 -->
<div id="clock" style="font-size: 18px; font-weight: bold; color: #ffffff; margin-top: 10px;"></div>
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
