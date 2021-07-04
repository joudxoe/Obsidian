客戶端 (JavaScript)
```
<script>
	function callbackFunction(data){
		document.getElementById('container').innerHTML=data;
	}
</script>
<script src="https://www.runoob.com/try/ajax/jsonp.php?callback=callbackFunction"></script>
```

客戶端 (jQuery)
```
$.getJSON('https://www.runoob.com/try/ajax/jsonp.php?callback=?', function(data){
	$('#container').html(data.result);	
});
```

客戶端 (jQuery)
```
$.ajax({
	type:'get',
	url:'http://flightQuery.com/jsonp/flightResult.aspx?code=CA1998',
	dataType:'jsonp',	
	jsonp:'callback',	// 用於獲取回調函數名的引數
	jsonpCallback:'flightHandler',	// 預設為jQuery自動生成的隨機函式名					
	success:function(data){
		$('#result').html('票價'+data.price+'元');
	},
	error:function(){
		// fail
	}
});
```

服務端
```
header('Content-type: application/json');
$callback=$_GET['callback'];	// 獲取回調函數名						
$data='["Jane","Sam"]';
echo $callback.'('.$data.')';	// 輸出JSON格式的數據						
```

---

客戶端
```
<script src="http://remoteserver.com/remote.js"></script>
<script>
	function callback(data){
		alert(data.name);
	}
</script>
```

remote.js
```
callback({	// 呼叫客戶端的callback函數並傳入JSON參數
	'name':'Jane',
	'age':24
});
```