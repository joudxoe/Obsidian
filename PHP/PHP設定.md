PHP設定
* `memory_limit` 允許配置多少記憶體，單位為位元組，預設為128MB
* `max_execution_time` PHP程式允許執行的時間，預設為30秒
* `short_open_tag` 是否允許使用PHP代碼短標籤
* `upload_max_filesize` 上傳檔案的最大限制
* `register_globals=On`

控制錯誤顯示的設定
* `display_errors`
* `error_reporting=E_ALL~E_NOTICE`
* `error_log`
* `html_erros`
* `log_erros`
* `display_startup_errors`
* `track_errors`

要點整理
- 限制程式執行時間，可有效避免單一網頁程式耗用太多伺服器資源