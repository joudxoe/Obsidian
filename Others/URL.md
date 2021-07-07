要點整理
- URL (Uniform/Universal Resource Locator - 統一資源定位器)

---

格式說明
- `scheme` <small>定義網路服務的類型/協議/通訊協定</small>
- `host` <small>主機名稱、子網域，默認主機是www</small>
- `domain` <small>網域名</small>
- `port` <small>主機上的網路埠號，http的默認端口是80</small>
- `path` <small>定義服務器上網站的根目錄路徑</small>
- `filename` <small>文檔名</small>
- `query-string` <small>查詢字串是以?開頭的資料，包含傳遞給伺服端處理的資料</small>
- `fragment-id` <small>片段識別符</small>

傳輸協議
- `http` <small>超文件傳輸協定，不加密</small>
- `https` <small>安全超文件傳輸協定，加密所有信息交換</small>
- `ftp` <small>文件傳輸協議，用於將文件下載或上傳至網站</small>
- `file` <small>本機文件</small>
- `mailto` <small>郵件協議、通過SMTP訪問</small>
- `tel` <small>電話協議</small>
- `sms` <small>簡訊協議</small>
- `ed2k` <small>ed2k下載鏈接協議</small>
- `thunder` <small>thunder下載鏈接協議</small>
- `flashget` <small>flashget下載鏈接協議</small>

---

```
# 語法規則
# scheme://host.domain:port/path/filename
# scheme://host:port/path?query-string#fragment-id
```