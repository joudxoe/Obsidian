AJAX
- AJAX是一種不需重整頁面，透過JavaScript和伺服器交換資料，來更新網頁內容的技術
- AJAX透過XHR發送HTTP請求，在不重整頁面的情況下，更新部份的網頁內容
- 更新頁面資料時不需進行頁面重載(Page Reload)，這種非同步更新資料的技術就是AJAX

同步請求
>客戶端會等待伺服端的回應才繼續下一步的動作，等待的期間無法處理其它事情，會導致頁面的阻塞，阻斷執行而造成卡死

非同步/異步請求
>客戶端不需等待伺服端的回應，瀏覽器仍可以持續處理其它工作，甚至繼續送出請求

AJAX請求的步驟
* 建立AJAX物件
* 發出請求
* 處理伺服器的回應

AJAX請求的方法
* GET
* POST
* PUT
* DELETE
* HEAD
* OPTIONS

要點整理
- send()方法的參數是請求訊息的payload內容，get方法不得送出payload，因此設為空值
- 設定請求時，預設使用非同步(async)的方式接受回應

*建立AJAX物件/XHR實例物件*
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

*發出請求*
```
xhr.open(請求類型，伺服器資源的URL，請求採用同步或非同步)
```

*請求外部公開資料*
```
var opendata='https://gank.io/api/random/data/%E7%A6%8F%E5%88%A9/20';
xhr.open('get',opendata,true);
```

*發送請求*
```
xhr.send(null);		// 暫時以null值代表請求中的資料
```

*處理伺服器回應/回調函式(callback)，讓回應完成時，能執行相對應處理的函式*
```
xhr.onreadystatechange=function(){
	if(xhr.readyState==4 && xhr.status==200){
		console.log(xhr.responseText);		
	}
}
```