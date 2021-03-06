要點整理
- HTTP狀態碼 (HTTP Status Code)是表示網頁伺服器回應超文字傳輸協定狀態的3位數代碼
- HTTP狀態碼是服務器對瀏覽器請求回應的三位數狀態代碼

---

成功
- `200` `OK` <small>HTTP請求成功</small>
- `201` `Created` <small>請求被創建完成，同時新的資源被創建</small>
- `202` `Accepted` <small>請求已被接受，但處理末完成</small>

重定向
- `301` `Moved Permanently` <small>請求的頁面已移轉至新的URL</small>
- `304` `Not Modified` <small>未按預期修改文檔</small>
- `307` `Temporary Redirect` <small>請求的頁面已臨時移轉至新的URL</small>

客戶端錯誤
- `400` `Bad Request` <small>錯誤的要求，語法錯誤服務器未能理解需求</small>
- `401` `Unauthorized` <small>需授權，被請求的頁面需要身份驗證，客戶端驗證失敗</small>
- `403` `Forbidden` <small>禁止，合法請求但禁止被請求頁面的訪問</small>
- `404` `Not Found` <small>找不到，服務器無法找到被請求的頁面</small>
- `405` `Method Not Allowed` <small>不允許的方法，請求中指定的方法不被允許</small>
- `406` `Not Acceptable` <small>伺服器返回的響應無法被客戶端所接受</small>
- `407` `Proxy Authentication Required` <small>需要Proxy驗證</small>
- `408` `Request Timeout` <small>要求逾時，請求超出了服務器的等待時間</small>
- `409` `Conflict` <small>衝突導致請求無法被完成</small>
- `410` `Gone` <small>已移除，被請求的頁面不可用</small>
- `415` `Unsupported Media Type` <small>不支援的媒體類型</small>
- `417`	`Expectation Failed` <small>預期失敗</small>
- `423` `Locked` <small>已鎖定</small>
- `424` `Failed Dependency` <small>失敗的相依性</small>

服務器錯誤
- `500` `Internal Server Error` <small>內部伺服器錯誤，服務器遇到不可預知的情況</small>
- `502` `Bad Gateway` <small>不正確的閘道，服務器收到無效的響應</small>
- `503` `Service Unavailable` <small>服務無法使用，服務器當前不可用，過載或當機</small>
- `504` `Gateway Timeout` <small>閘道逾時，服務器未能收到及時的響應</small>
- `505` `HTTP Version Not Supported` <small>不支援的HTTP版本</small>
- `507` `Insufficient Storage` <small>儲存空間不足</small>
- `511` `Network Authentication Required` <small>用戶需要提供身份驗證來獲取訪問權限</small>