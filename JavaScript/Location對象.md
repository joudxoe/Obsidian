要點整理
- Location對象包含當前URL的信息
- Location對象是Window對象的一部份，可通過window.location屬性對其進行訪問

---

Location對象方法
- `assign()` <small>載入新的文檔</small>
- `reload()` <small>重新載入當前文檔</small>
- `replace()` <small>用新的文檔替換當前文檔</small>

Location對象屬性
- `hash` <small>返回URL的錨，從#號開始的部份</small>
- `host` <small>返回URL的主機名和端口</small>
- `hostname` <small>返回URL的主機名</small>
- `href` <small>返回完整的URL</small>
- `pathname` <small>返回URL路徑名</small>
- `port` <small>返回URL使用的埠號/端口號</small>
- `protocol` <small>返回URL協議</small>
- `search` <small>返回URL的查詢字串，從?號之後的部份</small>