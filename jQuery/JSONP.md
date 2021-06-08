要點整理
- JSONP (JSON with Padding)是解決跨網域限制的方法，可從其它域獲取資料，也就是跨網域存取 (CORS)
- 因為同源策略不允許跨網域的請求和存取，所以訪問不同域的數據需要使用JSONP
- JSONP可以解決AJAX辦不到的跨網域存取問題
- 同域是指頁面必須有相同的協定(Protocol)、埠號(Port)和域名(Domain)
- JSONP利用src屬性不阻止指向路徑的這個漏洞來逃避同源策略
- JSONP傳遞一個回調引數給服務端，服務端返回資料將callback引數做為函式包住JSON資料供客戶端處理

jQuery實現JSONP的方式
- `$.getJSON`
- `$.ajax`