PHP設定
* `short_open_tag` <small>是否允許使用PHP代碼短標籤`<? ... ?>`</small>
* `register_globals=Off` <small>是否將EGPCS變數註冊為全域變數/全局變量</small>
* `output_buffering=Off` <small>輸出緩存允許在輸出內容後發送header標頭</small>
* `date.timezone=asia/taipei` <small>設定時區</small>
* `precision` <small>浮點數顯示時的有效位數</small>
* `safe_mode` <small>是否啟用安全模式</small>
* `post_max_size=4M` <small>PHP能接收POST資料的最大值</small>
* `magic_quotes_gpc` <small>是否對GET/POST/Cookie資料啟用[[魔術引號]]</small>

資源限制
* `memory_limit` <small>腳本可使用的記憶體，單位為位元組，預設為128MB</small>
* `max_execution_time` <small>PHP程式允許執行的時間，預設為30秒</small>
* `max_input_time` <small>腳本的最大資料讀取時間，以秒為單位</small>
* `upload_max_filesize` <small>上傳檔案的最大限制</small>

控制錯誤和記錄
* `display_errors` <small>在網頁上是否顯示錯誤，開發階段除錯建議打開</small>
* `error_reporting` <small>設定顯示的[[錯誤級別]]</small>
* `error_reporting=E_ALL & ~E_NOTICE` <small>顯示所有的錯誤，除了提醒</small>
* `error_log=filename` <small>使用指定的檔案記錄錯誤日誌</small>
* `html_erros` <small>是否在錯誤訊息中包含HTML語法錯誤</small>
* `log_erros` <small>在日誌檔案中記錄錯誤</small>
* `display_startup_errors` <small>若不是在Debug，建議關閉此項</small>
* `error_prepend_string` <small>指定輸出錯誤前的字串</small>
* `error_append_string` <small>指定輸出錯誤後的字串</small>

檔案上傳
* `file_uploads` <small>是否允許以HTTP方式上傳檔案</small>
* `upload_tmp_dir` <small>以HTTP方式上傳檔案的臨時目錄</small>
* `upload_max_filesize=2M` <small>允許上傳檔案的最大值</small>
* `default_socket_timeout` <small>預設連接超時時間，以秒為單位</small>
* `allow_url_fopen` <small>是否允許把URLs當做檔案處理</small>

郵件設定
* `SMTP`
* `smtp_port`
* `sendmail_from`

要點整理
- 限制程式執行時間，可有效避免單一網頁程式耗用太多伺服器資源