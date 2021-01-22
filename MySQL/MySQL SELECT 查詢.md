**使用`SELECT`語句在資料庫表中選記錄**

```
$sql="SELECT * FROM students";
```

*程序導向*
```
$result=mysqli_query($link,$sql);
if(mysqli_num_rows($result)>0){
	while($row=mysqli_fetch_array($result)){
		printf('%s',$row['name']);
	}
	// free result
	mysqli_free_result($result);
}
// close connection
mysqli_close($link);
```

*物件導向*
```
$result=$mysqli->query($sql);
if($result->num_rows>0){
	while($row=$result->fetch_array()){
		printf('%s',$row['name']);
	}
	// free result
	$result->free();
}
// close connection
$mysqli->close();
```

*資料物件*
```
$result=$pdo->query($sql);
if($result->rowCount()>0){
	while($row=$result->fetch()){
		printf('%s',$row['name']);
	}
	// free result
	unset($result);
}
// close connection
unset($pdo);
```