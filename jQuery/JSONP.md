要點整理
- JSONP (JSON with Padding)是JSON的一種使用模式，可以從別的域名獲取資料，也就是跨網域存取
- 因為同源策略不允許跨網域的請求和存取，所以訪問不同域的數據需要使用JSONP

---

```
$.getJSON('https://www.runoob.com/try/ajax/jsonp.php?jsoncallback=?',function(data){
	var result='';
	$('#container').html(result);
});
```