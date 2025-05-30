# 🌍 探索，是人类的本能。


### 🧾 一言
<script src="https://v1.hitokoto.cn/?encode=js&select=%23hitokoto" defer></script>
<div id="hitokoto">正在加载一言...</div>

### 🌐 访客信息
- **IP 地址**：<span id="ip"></span>
- **地理位置**：<span id="location"></span>

<div align="center">
  <iframe width="100%" height="200" src="https://ip.skk.moe/simple" frameborder="1"></iframe>
</div>

<script>
  // Display current date
  const today = new Date().toISOString().split('T')[0];
  document.getElementById("today-date").textContent = today;

  // Fetch and display lunar date
  fetch("https://www.36jxs.com/api/Commonweal/almanac?sun=" + today)
    .then(response => response.json())
    .then(data => {
      document.getElementById("lunar-date").textContent = data.data.lunar;
    })
    .catch(() => {
      document.getElementById("lunar-date").textContent = "获取失败";
    });

  // Fetch and display IP and location
  fetch("https://ipapi.co/json/")
    .then(response => response.json())
    .then(data => {
      document.getElementById("ip").textContent = data.ip;
      document.getElementById("location").textContent = `${data.city}, ${data.region}, ${data.country_name}`;
    })
    .catch(() => {
      document.getElementById("ip").textContent = "获取失败";
      document.getElementById("location").textContent = "获取失败";
    });
</script>
