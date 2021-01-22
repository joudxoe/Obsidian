*JSON是一種資料交換格式*

*資料交換格式是一種文字格式，在不同平台間交換資料，JSON是WEB應用中最流行通用*

***

*JSON物件*
```
{
	"book": {
		"name": "Harry Potter and the Goblet of fire",
		"author": "J. K. Rowling",
		"year": 2000,
		"genre": "Fantasy Fiction",
		"bestseller": true
	}
}
```

*JSON陣列*
```
{
	"fruits": ["apple","mango","banana","strawberry"]
}
```


*JSON編碼: 將關聯陣列編碼為JSON物件*
```
$scores=array('Peter'=>84,'Jane'=>92,'Sam'=>88);	// an associative array
json_encode($scores);
```

*JSON編碼: 將數值陣列編碼為JSON陣列*
```
$employees=['jane','same','peter','方大同'];	// an indexed array
json_encode($employees);
json_encode($employees, JSON_FORCE_OBJECT);	// 強制返回JSON物件
json_encode($employees, JSON_UNESCAPED_UNICODE);	// 不編碼中文
```

*JSON編碼: 將PHP物件編碼為JSON物件*
```
class Employee{
	public $name='jane';
	public $email='jane@gmail.com';
}
$jane=new Employee();
json_encode($jane);
```

*JSON解碼: 將JSON物件解碼/轉換為PHP物件*
```
$json={"Peter":84,"Jane":92,"Sam":88};
json_decode($json);
json_decode($json, true);	// 將JSON物件解碼為關聯陣列
```