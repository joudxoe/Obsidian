要點整理
- JSONP (JSON with Padding)是解決跨網域限制的方法，可從其它域獲取資料，也就是跨網域存取 (CORS)
- 因為同源策略不允許跨網域的請求和存取，所以訪問不同域的數據需要使用JSONP

---

```
$.getJSON('https://www.runoob.com/try/ajax/jsonp.php?jsoncallback=?',function(data){
	var result='';
	$('#container').html(result);
});
```