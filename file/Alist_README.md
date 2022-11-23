<FORM METHOD=GET ACTION=/search >             
<input type="text" name="box" placeholder=" 输入搜索关键词，Enter 键提交"  >         
<input type="hidden" name="url"> 
</FORM>   
<script>
    let searchObj = document.querySelector(".markdown-body form")
    let headRight = document.querySelector(".header-right")
    headRight.prepend(searchObj)
    searchObj.querySelector('input').style.width="100%"
</script>
<div align="center"><iframe width=100% height=50% src="https://ip.skk.moe/simple" frameborder="1px"></iframe></div>
