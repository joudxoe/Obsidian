要點整理
- `$.get()`使用HTTP GET方法生成Ajax請求

---

```
$.get(URL,data,success);
```

```
$.get('time.php',function(data){
	$('#result').html(data);
});
```