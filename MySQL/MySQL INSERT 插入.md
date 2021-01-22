**使用`INSERT INTO`語句插入資料到資料表**

*插入單行*
```
$sql="INSERT INTO students (name,email) VALUES ('jane','jane@gmail.com')";
```

*插入多行*
```
$sql="INSERT INTO students (name,email) VALUES 
	('jane','jane@gmail.com'),
	('sam','sam@gmail.com'),
	('lily','lily@gmail.com')";
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