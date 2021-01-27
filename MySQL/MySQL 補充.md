*SQL是用來操作/管理/維護資料庫的語言*

*XAMPP: Apache+MariaDB+PHP+Perl*

*列舉屬於文字資料型態，只能從固定的選項內挑選，ENUM為單選項，SET為複選項*

*SQL的敘述分為三大類: DDL、DML、DCL*

*DDL(資料定義語言) - 用來建立或刪除資料庫及資料表*
- CREATE: 建立資料庫或資料表
- DROP: 刪除資料庫或資料表
- ALTER: 修改資料庫或資料表的結構

*DML(資料操作語言) - 查詢或修改資料表的記錄，也就是CRUD*
- SELECT: 查詢資料表記錄
- INSERT: 新增資料表記錄
- UPDATE: 更新資料表記錄
- DELETE: 刪除資料表記錄

*DCL(資料控制語言) - 用來確認或取消資料庫執行的變更動作*
- COMMIT: 確認對資料庫執行的變更動作
- ROLLBACK: 取消對資料庫執行的變更動作
- GRANT: 賦予使用者操作權限
- REVOKE: 徹銷使用者的操作權限

*查詢敘述的基本語法*
```
	SELECT 欄位
	FROM 表格
	WHERE 查詢條件
	GROUP BY 分組設定
	HAVING 分組條件
	ORDER BY 排序設定
	LIMIT 限制設定
```

*其它條件運算子*
- BETWEEN AND
- IN()
- IS
- NOT
- IS NOT
- LIKE

*SQL函數類型*
- 數學函數: 計算數值的函數
- 字串函數: 操作字串的函數
- 日期函數: 操作日期的函數
- 轉換函數: 轉換資料型別或內容值的函數
- 彙總函數: 統計資料的函數