*程序導向*
```
$last_id=mysqli_insert_id($link);
```

*物件導向式*
```
$last_id=$msyqli->insert_id;
```

*資料物件*
```
$last_id=$pdo->lastInsertId();
```