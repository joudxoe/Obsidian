要點整理
- Linux是開放源始碼的類Unix作業系統，廣泛的運用於伺服器和嵌入式系統中
- Linux發佈版本(Linux distributions)是指可完整安裝使用的套件版本

主流的Linux發佈版本
- CentOS
- Fedora
- Ubuntu
- Debian

檔案與目錄管理指令
- `ls` <small>列出檔案和目錄</small>
- `pwd` <small>顯示當前工作目錄</small>
- `cd` <small>切換目錄</small>
- `mkdir` <small>新建資料夾</small>
- `cp` <small>複製檔案</small>
- `mv` <small>移動檔案或是重新命名</small>
- `rm` <small>刪除檔案</small>
- `rmdir` <small>刪除空目錄</small>
- `touch` <small>新增空白檔案</small>
- `cat` <small>顯示檔案內容</small>
- `tail` <small>顯示檔案最後幾行的內容</small>
- `more` <small>分頁顯示檔案內容</small>
- `file` <small>檢查檔案類型</small>

編輯文字檔案
- `nano`
- `vim`

檔案權限設定
- `chmod` <small>修改檔案權限</small>
- `chown` <small>修改檔案擁有者與群組</small>

系統管理
- `sudo` <small>使用最高權限執行指令</small>
- `su` <small>輸入root密碼後可暫時取得root權限</small>
- `kill`
- `killall`
- `who` <small>顯示目前使用者</small>
- `ps` <small>查看系統中正在執行的程序</small>
- `top` <small>查看系統狀態</small>
- `fsck` <small>檢查、修復Linux系統</small>

網路管理
- `ping`
- `traceroute` <small>路由追蹤</small>
- `nslookup` <small>查詢DNS回應是否正常</small>
- `netstat` <small>查詢網路狀況</small>
- `telnet` <small>遠端登入</small>

其它指令
- `man` <small>查詢某個指令的輔助說明</small>
- `help` <small>查詢某個內建指令的說明</small>
- `whatis` <small>查詢某個指令的用途</small>
- `find` <small>查詢檔案</small>
- `grep` <small>文件字串搜尋</small>
- `at`
- `crontab` <small>例行性工作排程</small>
- `clear` <small>清除螢幕</small>

套件管理
- 更新套件
	```
	$ sudo 套件名稱 update
	```
- 升級並下載套件
	```
	$ sudo 套件名稱 upgrade
	```
- 安裝套件
	```
	$ sudo 套件名稱 install fortune
	```
- 移除套件
	```
	$ sudo 套件名稱 remove forturn
	```