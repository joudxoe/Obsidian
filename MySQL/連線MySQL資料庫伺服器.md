*程序導向*
```
$link=mysqli_connect('hostname','username','password','database');
if($link===false) die(mysqli_connect_error());
mysqli_close($link);
```

*物件導向*
```
$mysqli=new mysqli('hostname','username','password','database');
if($mysqli===false) die($mysqli->connect_error);
$mysqli->close();
```

*資料物件(PDO)*
```
try{
	// attemp mysql server connection
	$pdo=new PDO('mysql:host=hostname;dbname=database','root','password');
	// set the PDO error mode to exception
	$pdo->setAttribute(PDO::ATTR_ERRMODE,PDO::ERRMODE_EXCEPTION);
}catch(PDOException $e){
	die($e->getMessage());
}
// close connection
unset($pdo);
```