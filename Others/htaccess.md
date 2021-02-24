.htaccess是Apache Web Server對系統目錄進行權限規則設置的一個配置文件

常應用的功能
* 定義默認首頁
* 404
* 301轉向/重導向/重定向
* 偽靜態/網址改寫
* 限制圖片外鏈
* 限制下載
* 密碼保護
* 去除頁面廣告

初始設定
```
<IfModule mod_rewrite.c>
RewriteEngine On
RewriteBase /
RewriteRule . /index.php [L]
</IfModule>
```


變更默認首頁
```
DirectoryIndex default.html
```

自定義錯誤頁面
```
ErrorDocument 404 /error/404.html
ErrorDocument 503 /error/503.html
```

頁面跳轉
```
Redirect home.html index.html
```

301重新導向
```
Redirect 301 / https://newsite.com
Redirect 301 /arts/index.html /news/index.html
Redirect 301 /old.html https://website.com/new.html
```

禁止特定IP
```
Order allow,deny
Deny from 145.186.144.122
Deny from 124.15
Allow from all
```

禁止瀏覽目錄
```
Options All -Indexes
```

補充資料
1. 一般會將.htaccess文件放在網站的根目錄，以控制所在目錄及所有子目錄
2. 301常被用於網址發生變化時，例如變更網域、網站目錄或是頁面名稱


