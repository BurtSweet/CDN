# 🌍 欢迎来到我的 Alist 网盘

> “探索，是人类的本能。”

---

## 📅 今日日期：<span id="today-date"></span>
<script>
  document.getElementById("today-date").textContent = new Date().toLocaleDateString();
</script>


---

### 🧾 一言
<script src="https://v1.hitokoto.cn/?encode=js&select=%23hitokoto" defer></script>
<div id="hitokoto">正在加载一言...</div>


---

### 🌐 访客信息
- **IP 地址**：<span id="ip"></span>
- **地理位置**：<span id="location"></span>
<script>
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

<div align="center">
  <iframe width="100%" height="200" src="https://ip.skk.moe/simple" frameborder="1"></iframe>
</div>
