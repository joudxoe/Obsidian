要點整理
- AJAX (Asynchronous JavaScript and XML - ==非同步==的JavaScript與XML)
- AJAX是一種不需重整頁面，透過JavaScript和伺服器交換資料，來更新網頁內容的技術
- AJAX透過XHR發送HTTP請求，在不需重整/刷新頁面的情況下，更新部份的網頁內容
- AJAX是一種將資料從伺服器載入到瀏覽器而無需重新載入整個頁面的方法
- AJAX是一種與服務器交換數據的技術，可以在不重新載入頁面的情況下更新部份網頁的內容
- AJAX通過JavaScript非同步從Web伺服器交換資料，而無需重新整理頁面
- 更新頁面資料時不需進行頁面重載(Page Reload)，這種非同步更新資料的技術就是AJAX
- 實現客戶端的異步請求操作，在不刷新頁面的情況下與服務器通信，減少用戶的等待時間
- 不同的瀏覽器以不同的方式實做AJAX，JS必須編寫不同的AJAX程式碼以確保AJAX能跨瀏覽器運行

---

AJAX請求的步驟
* 建立AJAX物件
* 發出請求
* 處理伺服器的回應

---

同步請求
- 客戶端會等待伺服端回應才繼續下一動作，等待時因無法處理其它事情會導致頁面阻塞，阻斷執行造成卡死

非同步/異步請求
- 客戶端不需等待伺服端的回應，瀏覽器仍可以持續處理其它工作，甚至繼續送出請求
