要點整理
- cookie是一種將資料儲存在客戶端/瀏覽器的技術
- cookie主要用來記錄使用者資訊，例如:會員登入、購物車，瀏覽記錄等
- 由於cookie是儲存在用戶端的電腦上，有被竊取的風險，重要的資訊應採用session儲存
- 刪除cookie只要將變數值給空值，並設定一個過期/失效的時間即可

使用cookie的限制
* 必須在HTML內容輸出之前設定
* cookie不能超過4KB

啟用cookie
```
setcookie('user','Jane',time()+3600);
```

讀取cookie
```
echo $user;
```

```
echo $_COOKIE['user'];
```

```
echo $HTTP_COOKIE_VARS['user'];
```

刪除cookie
```
setcookie('user','',time()-1);
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