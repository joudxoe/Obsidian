要點整理
- Composer是一套PHP==函式庫相依性管理工具==
- 套件可能會引用到其它套件的物件或函式，於是套件之間產生相依性
- 在專案中記錄和管理套件之間交互引用的關係稱為相依管理
- 將vendor目錄加入`.gitignore`中，套件不需要被commit
- composer.json是一個json資料格式的設定檔，記錄安裝的套件及版本
- composer.lock會明確列出專案用到的套件及版本，確保其它人都使用相同的版本號的套件
- composer.lock不可手動建立，會在執行install或update時自動產生及更新
- 若有手動更新composer.json，需要執行update同步composer.json和composer.lock
- 版本號的組成: `主版本號` . `副版本號` . `修正版本號`
- 執行完安裝指令後會有composer.json、composer.lock和vendor目錄，安裝的套件會放在vendor目錄

---

INSTALL使用時機
- install會先找composer.lock，若檔案存在則依其中指定的版本安裝，若不存在則讀取composer.json來安
	裝並產生composer.lock

- 若是從其它處拿到專案(例如github)，且專案目錄中已有composer.lock，最安全的作法是使用install，這樣
	可以確保安裝的套件版本和原專案的開發是相同的版號
	
---

UPDATE使用時機
- update會去讀取composer.json，並安裝最新版本，同時更新composer.lock
- 當有確定要更新套件版本或是第一次下載套件時，才用update
- 使用update的風險在於，可能會安裝到最新的版本造成程式執行時因為不相容而發生錯誤