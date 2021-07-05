要點整理
- 使用PHPMailer時，PHP必須安裝OpenSSL的擴充程式

---

安裝PHPMailer套件
```
composer require phpmailer/phpmailer
```

發送郵件
```
include 'PHPMailerAutoload.php';	// 引入PHPMailer類別
mb_internal_encoding('UTF-8');		// 寄信有亂碼則加上這一行
$mail=new PHPMailer();				// 建立PHPMailer物件
$mail->IsSMTP();					// 設定使用SMTP寄信
$mail->SMTPAuth=true;				// 設定SMTP需要驗證
$mail->SMTPSecure='ssl';			// SMTP使用SSL連線
$mail->Host='ssl://smtp.gmail.com';	// 設定SMTP主機
$mail->Port=465;					// Gmail的SMTP埠位為465或587
$mail->CharSet='big5';				// 設定郵件編碼
$mail->Username='';
$mail->Password='';
$mail->From='';
$mail->FromName='測試人員';
$mail->Subject='';					// 郵件標題
$mail->Body='';						// 郵件內容
$mail->IsHTML(true);				// 郵件內容是否為HTML
$mail->AddAddress('jane@gmail.com','Jane');		// 設定收件者郵件及名稱
if(!$mail->Send()){
	printf('郵件發送錯誤: %s',$mail->ErrorInfo);
}else{
	echo '郵件發送完成';
}
```

```
require 'PHPMailer/PHPMailer.php';
$mail=new PHPMailer();
try{
	// Server settings
	$mail->SMTPDebug=2;
	$mail->isSMTP();
	$mail->Host='ssl://smtp.gmail.com';
	$mail->SMTPAuth=true;
	$mail->Username='';
	$mail->Password='';
	$mail->SMTPSecure='ssl';	
	$mail->Port=465;	
	// Recipients
	$mail->setFrom('admin@domain.com','admin');
	$mail->AddAddress('jane@gmail.com','Jane');
	// Content
	$mail->isHTML(true);
	$mail->Subject=iconv('big5','utf-8','信件標題');
	$mail->Body='';
	$mail->send();
	echo '郵件發送完成';
}catch(Exception $e){
	echo 'Error: '.$mail->ErrorInfo;
}
```