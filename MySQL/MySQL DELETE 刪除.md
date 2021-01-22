**使用`DELETE`語句刪除資料庫表中的記錄**

```
$sql="DELETE FROM students WHERE name='jane'";
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