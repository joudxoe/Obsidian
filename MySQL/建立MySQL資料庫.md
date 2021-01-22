**使用 ` CREATE DATABASE `語句建立資料庫**

```
$sql="CREATE DATABASE company";
```

*程序導向*
```
$result=mysqli_query($link,$sql);
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
	echo $e->getMessage();
}
```

