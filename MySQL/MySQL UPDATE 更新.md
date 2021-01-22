**使用`UPDATE`語句更新資料庫表中的記錄**

```
$sql="UPDATE students SET email='jane@hotmail.com' WHERE name='jane'";
```

*程序導向*
```
$result=mysqli_query($link, $sql);
if(!$result) die(mysqli_error($link));
```

*物件導向*
```
$result=$mysqli->query($sql);
if(!$result) die($mysqli->error);
```

*資料物件*
```
try{
	$pdo->exec($sql);
}catch(PDOException $e){
	die($e->getMessage());
}
```