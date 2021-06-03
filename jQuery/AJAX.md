AJAX方法
- `$.ajax()` <small>執行異步AJAX請求</small>
- `$.ajaxSetup()` <small>為AJAX請求設置默認值</small>
- `$.param()` <small>建立數組或對象的序列化表示形式，可用於AJAX請求的URL查詢字符串</small>
- `ajaxComplete()` <small>設定AJAX請求完成時執行的函數</small>
- `ajaxError()` <small>設定AJAX請求失敗時執行的函數</small>
- `ajaxSend()` <small>設定AJAX請求發送之前執行的函數</small>
- `ajaxStart()` <small>設定第一個AJAX請求開始時執行的函數</small>
- `ajaxStop()` <small>設定所有的AJAX請求完成時運行的函數</small>
- `ajaxSuccess()` <small>設定AJAX請求成功時運行的函數</small>
- `serialize()` <small>將序列化表單值編碼為URL查詢字符串</small>
- `serializeArray()` <small>將序列化表單值編碼為關聯陣列</small>

要點整理
- ==同源策略==基於安全性的考量，不允許跨來源的請求和存取，可避免自已網站的資源被存取或修改