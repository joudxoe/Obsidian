要點整理
- cookie是一種將資料==儲存在客戶端/瀏覽器==的技術
- cookie主要用來==記錄使用者資訊/識別用戶==，例如:會員登入、購物車，瀏覽記錄等
- 由於cookie是儲存在用戶端的電腦上，有被竊取的風險，重要的資訊應採用session儲存
- 刪除cookie只要將變數值給空值，並設定一個過期/失效的時間即可
- cookie是HTTP標頭的組成部份，而標頭必須在其它頁面內容發送之前最先輸出
- 在setcookie()函數前輸出HTML標籤，echo語句，甚至空行都會導致出錯
- 若未設置cookie過期時間，則在關閉瀏覽器時自動刪除cookie數據

---

使用cookie的限制
* 必須在HTML內容發送之前設定輸出cookie
* cookie不能超過4KB

---

setcookie()函數的參數說明
- `name` - cookie的變數名
- `value` - cookie的變數值
- `expire` - cookie的失效時間
- `path` - cookie在服務器端的有效路徑
- `domain` - cookie有效的域名
- `secure` - 指定cookie是否通過https安全連接

---

setcookie()函數的參數
```
setcookie(name,value,expire,path,domain,secure);
```

啟用cookie
```
// 設置過期時間為一個月(60秒*60分*24時*30天)
$expire=time()+60*60*24*30;
setcookie('user','Jane',$expire);
```

讀取cookie
```
echo $user;
echo $_COOKIE['user'];
echo $HTTP_COOKIE_VARS['user'];
```

刪除cookie
```
setcookie('user','',time()-1);
setcookie('user','',0);
```

設定多個同名的cookie，要用陣列
```
setcookie("user['name']",'Jane');
setcookie("user['gender']",'Female');
```

讀取cookie陣列
```
echo $user['name'];
```