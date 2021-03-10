要點整理
- Smatry是PHP最為流行的範本引擎/模板引擎
- 模板引擎的目的在於==分離==程式邏輯(PHP)和呈現邏輯(HTML)

Smarty安裝
1. 到Smarty官網下載Smarty套件
2. 將解壓縮後的libs目錄放到根目錄下

Smarty環境設定
```
define('SMARTY_DIR','smarty-2.6.9')
define('__SITE_ROOT','d:/appserv/www/project');

include 'libs/Smarty.class.php';
require_once SMARTY_DIR.'/Smarty.class.php';

$tpl=new Smarty();
$tpl->template_dir=__SITE_ROOT.'/templates/';
$tpl->compile_dir=__SITE_ROOT.'/templates_c/';
$tpl->config_dir=__SITE_ROOT.'/configs/';
$tpl->cache_dir=__SITE_ROOT.'/cache/';

$tpl->caching=false;
$tpl->error_reporting=E_ALL;
$tpl->debugging=true;
$tpl->left_delimiter='<{';
$tpl->right_delimiter='}>';
```