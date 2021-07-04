要點整理
- Smatry是PHP最為流行的範本/模板引擎
- 模板引擎的目的在於==分離==程式邏輯(PHP)和呈現邏輯(HTML)
- Smarty的開發模式也是以[[MVC]]架構為概念

---

Smarty安裝
1. 到Smarty官網下載Smarty套件
2. 將解壓縮後的libs目錄放到根目錄下

Smarty方法
- `assign()` <small>在模板執行時賦值給模板變數</small>
- `display()` <small>用於顯示模板</small>

---

Smarty環境設定
```
# 定義服務器根目錄的絕對路徑
# define('BATH_PATH'$_SERVER['DOCUMENT_ROOT']);
# 定義網站目錄
# define('__SITE_ROOT','d:/appserv/www/project');
# 定義Smarty目錄的絕對路徑
# define('SMARTY_DIR','smarty-2.6.9');
# include 'libs/Smarty.class.php';	
# 加載Smarty類庫文件
# require_once SMARTY_DIR.'/Smarty.class.php';
# $tpl=new Smarty();	// 實例化Smarty對象
# 定義模板目錄的路徑
# $tpl->template_dir=__SITE_ROOT.'/templates/';
# 定義編譯目錄的路徑
# $tpl->compile_dir=__SITE_ROOT.'/templates_c/';
# 定義配置目錄的路徑
# $tpl->config_dir=__SITE_ROOT.'/configs/';
# 定義緩存目錄的路徑
# $tpl->cache_dir=__SITE_ROOT.'/cache/';
# 關閉緩存
# $tpl->caching=false;
# 打開調試除錯功能
# $tpl->debugging=true;
# 定義定界符
# $tpl->left_delimiter='<{';
# 定義定界符
# $tpl->right_delimiter='}>';
# $tpl->error_reporting=E_ALL;
```