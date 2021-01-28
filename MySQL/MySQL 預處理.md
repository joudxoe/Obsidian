預處理語句是一個包含佔位符而不是實際SQL語法的查詢模板，佔位符會在執行時被實際值替換

使用預處理句的優點

* 預處理語句可以高效率的重覆執行相同的語句，通過傳遞不同的引數執行多次
* 減少了伺服器頻寬的使用，因為每一次執行時只需傳送佔位符值而不是完整的SQL語句
* 提供SQL注入保護，因為佔位符的值不直接嵌入SQL查詢字串中

```
$sql="INSERT INTO students (name,email) VALUES (?,?)";
```

*程序導向*
```
$stmt=mysqli_prepare($link,$sql);
if(!$stmt) die(mysqli_error($link));
// bind variables to the prepared statement as parameters
mysqli_stmt_bind_param($stmt,'ss',$name,$email);
// set the parameters values and execute
$name='jane';
$email='jane@gmail.com';
mysqli_stmt_execute($stmt);
$name='sam';
$email='sam@gmail.com';
mysqli_stmt_execute($stmt);
// close statement
mysqli_stmt_close($stmt);
// close connection
mysqli_close($link);
```

*物件導向*
```
$stmt=$mysqli->prepare($sql);
if(!$stmt) die($mysqli->error);
// bind variables to the prepared statement as parameters
$stmt->bind_param('ss',$name,$email);
// set the parameters values and execute
$name='jane';
$email='jane@gmail.com';
$stmt->execute();
// close statement
$stmt->close();
// close connection
$mysqli->close();
```

*資料物件*

```
try{
	$sql="INSERT INTO students (name,email) VALUES (:name,:email)";
	$stmt=$pdo->prepare($sql);
	// bind parameters to statement
	$stmt->bindParam(':name',$name,PDO::PARAM_STR);
	$stmt->bindParam(':email',$email,PDO::PARAM_STR);
	// set the parameters values and execute
	$name='jane';
	$email='jane@gmail.com';
	$stmt->execute();
}catch(PDOException $e){
	die($e->getMessage());
}
// close statement
unset($stmt);
// close connection
unset($pdo);
```

*繫結變數的資料型別: bdis*