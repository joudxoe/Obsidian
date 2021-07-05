要點整理
- PDO是存取資料庫的延伸函式庫

---

PDO的好處
- PDO為物件導向設計
- PDO為PHP存取資料庫定義了一致性的介面，提供了一個資料存取抽象層
- PDO將存取資料庫的動作抽象化，使用一致的方式存取處理不同類型資料庫的資料
- 可避免SQL注入(SQL Injection)

檢查PDO是否啟用
* 檢查PHP版本的擴充功能目錄是否有內建PDO擴充元件
* 通過phpinfo()查看是否啟用/安裝PDO擴充功能
* 啟用PDO類別庫，將PHP初始設定檔關於PDO類別庫前面的註釋符號去掉

---

```
# 啟用PDO類別庫

# extension=php_pdo.dll

# extension=php_pdo_mysql.dll
```