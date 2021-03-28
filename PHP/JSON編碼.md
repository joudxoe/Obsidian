將關聯陣列編碼為JSON物件
```
$scores=array('Peter'=>84,'Jane'=>92,'Sam'=>88);
json_encode($scores);
```

將數值陣列強制編碼為JSON物件
```
$employees=['jane','sam','peter'];
json_encode($employees, JSON_FORCE_OBJECT);
```

將數值陣列編碼為JSON陣列
```
$employees=['jane','sam','peter'];
json_encode($employees);
```

將含有中文的陣列轉成JSON物件
```
$city=array(
	'北部'=>'台北','北部'=>'桃園',
	'中部'=>'台中','中部'=>'南投',
	'南部'=>'台南','南部'=>'高雄'
);
// 利用urlencode編碼中文字
foreach($city as $key=>$val){
	$new_city[urlencode($key)]=urlencode($val);
}
// 將資料轉成JSON格式
$json=json_encode($new_city);
// 使用urldecode將資料轉回中文
$data=urldecode($json);
```

將PHP物件編碼為JSON物件
```
class Employee{
	public $name='jane';
	public $email='jane@gmail.com';
}
$jane=new Employee();
json_encode($jane);
```