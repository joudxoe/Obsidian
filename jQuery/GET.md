AJAX方法
- `$.get()` <small>使用HTTP GET請求從服務器加載數據</small>
- `$.getJSON()` <small>使用HTTP GET請求從服務器加載JSON編碼的數據</small>
- `$.getScript()` <small>使用AJAX的HTTP GET請求從服務器加載並執行JavaScript</small>

要點整理
- GET主要用於從服務器獲取數據，可能返回緩存數據

---

```
$.get(URL,success);
```

```
$.get('time.php',function(data){
	$('#result').html(data);
});
```

```
$.get('time.php',function(data,status){
	if(status=='success')
		$('#result').html(data);
});
```