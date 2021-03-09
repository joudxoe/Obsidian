要點整理
- session是儲存在何服器端，用來儲存/記錄使用者資訊
- session_start()必須放在程式的最開頭，在還沒輸出任何東西之前，位於HTML標籤之前

常用的session函式庫

`session_start()`
`session_destroy()`
`session_name()`
`session_module_name()`
`session_sava_path()`
`session_id()`
`sesson_register()`
`session_unregister()`
`session_is_registered()`
`session_decode()`
`session_encode()`

啟用session
```
session_start();
```

設定session
```
$_SESSION['author']='Jane';
```

取得session的值
```
echo $_SESSION['author'];
```

刪除指定的session
```
unset($_SESSION['author']);
```

刪除全部的session，需謹愼使用
```
session_destroy();
```

```
session_unset();
```