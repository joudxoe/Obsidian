JSON編碼: 將關聯陣列編碼為JSON物件
```
$scores=array('Peter'=>84,'Jane'=>92,'Sam'=>88);	// an associative array
json_encode($scores);
```

JSON編碼: 將數值陣列編碼為JSON陣列
```
$employees=['jane','same','peter','方大同'];	// an indexed array
json_encode($employees);
json_encode($employees, JSON_FORCE_OBJECT);	// 強制返回JSON物件
json_encode($employees, JSON_UNESCAPED_UNICODE);	// 不編碼中文
```

JSON編碼: 將PHP物件編碼為JSON物件
```
class Employee{
	public $name='jane';
	public $email='jane@gmail.com';
}
$jane=new Employee();
json_encode($jane);
```