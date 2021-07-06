要點整理
- URL編碼主要是對網址問號後面的查詢字串參數進行編碼
- URL編碼可用來==隱藏URL傳遞的參數==
- 對查詢字符串進行URL編碼，使用`urlencode()`函數
- 對URL編碼進行解碼，使用`urldecode()`函數
- urlencode()將空格編碼為`+`，rawurlencode()將空格編碼為`%20`

---

URL編碼函數
- `urlencode()` <small>針對URL中文字符的編碼轉化，中文編碼方式有GB2312和UTF-8</small>
- `urldecode()`
- `rawurlencode()`
- `rawurldecode()`

---

URL編碼
```
$query_string='foo='.urlencode($foo).'&bar='.urlencode($bar);
```