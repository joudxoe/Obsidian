PMA登入模式
- `http`
- `cookie`
- `config`

---

設定phpMyAdmin的目錄路徑
```
$cfg['PmaAbsoluteUri']='http://localhost/phpMyAdmin/';

$cfg['PmaAbsoluteUri']='http://140.128.51.220/phpMyAdmin/';
```

設定phpMyAdmin認證/登入模式
```
$cfg['Servers'][$i]['auth_type']='http';
```

設定phpMyAdmin使用者帳密
```
$cfg['Servers'][$i]['controluser']='root';
$cfg['Servers'][$i]['controlpass']='rootpass';
```

設定安裝phpMyAdmin的伺服器位址
```
$cfg['Servers'][$i]['host']='localhost';
$cfg['Servers'][$i]['contorlhost']='localhost';
```

更改連接MySQL的PORT，MySQL的預設PORT是3306
```
$cfg['Servers'][$i]]['port']=3306;
```

其它設定
```
$cfg['Servers'][$i]['connect_type']='tcp';

$cfg['Servers'][$i]['extension']='mysql';

$cfg['Servers'][$i]['compress']='false';
```