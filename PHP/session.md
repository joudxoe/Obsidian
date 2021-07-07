要點整理
- session是儲存在何服器端，用來儲存/記錄使用者資訊
- `session_start()`必須放在程式的最開頭，在還沒有輸出任何內容之前
- `session_register()`若無作用或提出警告，可能是PHP設定檔的`register_globals=Off`

---

PHP啟動會話的方式
- 通過`session_start()`函數啟動會話
- 通過`session_register()`函數創建會話

---

Session工作原理

- 啟動Session會話時，會生成一個隨機且唯一的session_id，id儲存在服務器的內存中，關閉頁面時id會自
	動註銷，重新登錄頁面時，會再次生成一個隨機且唯一的id

Session的功能

- 網頁是一種無狀態的連接程序，因此無法得知用戶的瀏覽狀態，session可用來記錄用戶訊息，以供用戶再
	次以此身份對WEB服務器提交驗證時做身份/用戶/帳密確認

---

啟用session
```
session_start();
```

註冊/設定session
```
$_SESSION['author']='Jane';
```

```
$HTTP_SESSION_VARS['author']='Jane';
```

```
$auhtor='Jane';
session_register('author');
```

取得session的值
```
echo $_SESSION['author'];
```

刪除指定的session
```
unset($_SESSION['author']);
```

```
$_SESSION['author']=null;
```

刪除全部的session，需謹愼使用
```
session_destroy();
```

```
$_SESSION=array();
```

```
session_unset();
```