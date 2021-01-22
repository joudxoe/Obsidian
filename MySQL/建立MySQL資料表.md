**使用`CREATE TABLE`語句建立資料表**

```
$sql="CREATE TABLE students(
	id INT(6) UNSIGNED AUTO_INCREMENT PRIMARY KEY,
	name varchar(20) NOT NULL,
	email varchar(80) NOT NULL UNIQUE
)";
```

```
NOT NULL - 必須有值，不能為空
UNSIGNED - 使用無符號數值，0及正數
```

*程序導向*
```
if(!mysqli_query($link,$sql)) die(mysqli_error($link));
```

*物件導向*
```
if(!$mysqli->query($sql)) die($mysqli->error);
```

*資料物件*
```
try{
	$pdo->exec($sql);
}catch(PDOException $e){
	die($e->getMessage());
}
```