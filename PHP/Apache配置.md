允許通過外網訪問，默認只允許本機訪問
```
#Deny from all
#Allow from 127.0.0.1
Allow from all
```

開啟URL重寫功能
```
#AllowOverride None
AllowOverride All
LoadModule rewrite_module modules/mod_rewrite.so
```

更改根目錄
```
DocumentRoot "C:/AppServ/www"
<Directory "C:/AppServ/www">
```

補充資料
- Apache設定檔若有變更，要記得==重啟Apache服務器==，設定才會生效