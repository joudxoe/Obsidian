建立AJAX物件/XHR實例物件
```
function getXHRObject(){
	var ajax=null;
	if(window.XMLHttpRequest){
		ajax=new XMLHttpRequest();
	}else if(window.ActiveXObject){
		ajax=new ActiveXObject('MSXML2.XMLHTTP.3.0');
	}
	return ajax;
}
var xhr=getXHRObject();
```

發出請求
```
xhr.open(請求類型，伺服器資源的URL，請求採用同步或非同步)
```

請求外部公開資料
```
var opendata='https://gank.io/api/random/data/%E7%A6%8F%E5%88%A9/20';
xhr.open('get',opendata,true);
```

發送請求
```
xhr.send(null);	 // 請求訊息的payload內容，get方法不得送出payload，因此以null值代表請求中的資料
```

處理伺服器回應/回調函式(callback)，讓回應完成時，能執行相對應處理的函式
```
xhr.onreadystatechange=function(){
	if(xhr.readyState==4 && xhr.status==200){
		console.log(xhr.responseText);		
	}
}
```