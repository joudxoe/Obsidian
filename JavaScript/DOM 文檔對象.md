要點整理
- 當瀏覽器載入文檔後，文檔便成為Document對象，Document對象是HTML文檔的根節點
- Document對象可以對HTML頁面中所有元素進行訪問/操作
- Document對象是Window對象的一部份，可通過window.document屬性對其進行訪問

---

Document對象方法
- `document.addEventListener()` <small>向文檔添加事件</small>
- `document.close()` <small>關閉用document.open()打開的輸出流</small>
- `document.createAttribute()` <small>創建屬性節點</small>
- `document.createComment()` <small>創建注釋節點</small>
- `document.createDocumentFragment()` <small>創建文檔碎片</small>
- `document.createElement()` <small>創建元素節點</small>
- `document.createTextNode()` <small>創建文本節點</small>
- `document.getElementsByClassName()` <small>返回帶有指定類名的所有元素的節點列表</small>
- `document.getElementById()` <small>返回帶有指定ID的元素</small>
- `document.getElementsByName()` <small>返回帶有指定名稱的所有元素的節點列表</small>
- `document.getElementsByTagName()` <small>返回帶有指定標籤名的所有元素的節點列表</small> 
- `document.importNode()` <small>複製節點到另一個文檔</small>
- `document.normalize()` <small>刪除空文本節點</small>
- `document.open()` <small>開啟一個輸出流收集輸出的內容</small>
- `document.querySelector()` <small>返回匹配選取器的第一個元素</small>
- `document.querySelectorAll()` <small>返回匹配選取器的所有元素的節點列表</small>
- `document.removeEventListener()` <small>移除文檔中的事件</small>
- `document.renameNode()` <small>重命名元素或者屬性節點</small>
- `document.write()` <small>對文檔寫入內容</small>
- `document.writeln()` <small>對文檔寫入內容後換行</small>

Document對象屬性
- `document.activeElement` <small>返回當前獲取焦點元素</small>
- `document.anchors` <small>返回文檔中所有錨點鏈接的數組</small>
- `document.baseURI` <small>返回文檔的基礎URI</small>
- `document.body` <small>返回文檔的body元素</small>
- `document.cookie` <small>設置或返回當前文檔的Cookie</small>
- `document.doctype` <small>返回文檔的文檔類型聲明 (DTD)</small>
- `document.documentElement` <small>返回文檔的根節點</small>
- `document.documentMode` <small>返回瀏覽器渲染文檔的模式</small>
- `document.documentURI` <small>設置或返回文檔的位置</small>
- `document.domain` <small>返回當前文檔的域名</small>
- `document.embeds` <small>返回文檔中所有嵌入內容的集合</small>
- `document.forms` <small>返回文檔中所有表單的集合</small>
- `document.images` <small>返回文檔中所有圖片的集合</small>
- `document.lastModified` <small>返回文檔最後被修改的日期和時間</small>
- `document.inputEncoding` <small>返回文檔的編碼方式</small>
- `document.implementation` <small>返回處理文檔的DOM Implementation對象</small>
- `document.links` <small>返回文檔中所有鏈接的數組</small>
- `document.readyState` <small>返回當前文檔的載入狀態</small>
- `document.referrer` <small>返回當前文檔的來源URL</small>
- `document.scripts` <small>返回頁面中所有腳本的集合</small>
- `document.strictErrorChecking` <small>設置或返回是否強制進行錯誤檢查</small>
- `document.title` <small>返回當前文檔的標題</small>
- `document.URL` <small>返回文檔完整的URL</small>