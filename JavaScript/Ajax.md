*AJAX是一種不需重整頁面，透過JavaScript和伺服器交換資料，來更新網頁內容的技術*

*同步請求*

*客戶端會等待伺服端的回應才會繼續下一步的動作，等待的期間無法處理其它事情*

*非同步請求*

*客戶端不需等待伺服端的回應，仍可以持續處理其它工作，甚至繼續送出請求*

*AJAX請求的步驟*
* 建立AJAX物件
* 發出請求
* 處理伺服器的回應

*建立AJAX物件*
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

*發送請求*
```
xhr.send(null);		// 暫時以null值代表請求中的資料
```

*處理伺服器回應*