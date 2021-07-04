要點整理
- POST常用於連同請求一併提交/更新數據

---

AJAX方法
- `$.post()` <small>通過HTTP POST請求向服務器提交數據</small>

---

```
$.post(URL,data,success);
```

```
$.post('form.php',{
	name:'Jane',
	gender:'Female'
},function(data,status){
	if(status=='success')
		$('#resut').html(data);
});
```