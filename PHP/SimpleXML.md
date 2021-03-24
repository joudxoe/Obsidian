PHP操作XML格式文檔的方法
- XML語法解析函數
- DOMXML函數
- SimpleXML函數 (PHP5新增)

創建SimpleXML對象的方法
- `simplexml_load_file($file)`
- `simplexml_load_string($str)`
- `simplexml_import_dom($dom)`

創建XML對象
```
header('content-type:text/html;charset=utf-8');
$xml=simplexml_load_file('toys.xml');
print_r($xml);
```

```
$str=<<<XML
<?xml version="1.0" encoding="utf-8"?>
<object>
	<book>
		<title>PHP從入門到精通</title>
	</book>
</object>
XML;
$xml=simplexml_load_string($str);
print_r($xml);
```

```
$dom=new domDocument();
$dom->loadXML($str);
$xml=simplexml_import_dom($dom);
print_r($xml);
```