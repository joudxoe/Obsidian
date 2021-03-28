將JSON物件解碼/轉換為PHP物件
```
$json={"Peter":84,"Jane":92,"Sam":88};
json_decode($json);
```

將JSON物件解碼為關聯陣列
```
$json={"Peter":84,"Jane":92,"Sam":88};
json_decode($json, true);
```
