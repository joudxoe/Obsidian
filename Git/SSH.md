要點整理
- 當本端透過SSH與GitHub連線時，會使用==RSA加密演算法==，RSA是一對金鑰，一把私鑰加一把公鑰
- SSH產生的金鑰有兩把，一把是新增到遠端倉庫/GitHub的公鑰，另一把是存放在本機的私鑰
- 金鑰代理是給有設定金鑰密碼的人，在每次使用金鑰時不需再輸入密碼

RSA驗證流程
1. 先在自已的本機產生一對RSA金鑰
2. 將公鑰提供給GitHub Server
3. 本端使用SSH與GitHub連線時，GitHub使用公鑰和本機的私鑰進行加密及身份認證

SSH連線運作方式
1. Client端發送SSH連線請求
2. Server端發送隨機訊息
3. Client端使用私鑰加密隨機訊息後並回傳加密訊息給Server端
4. Server端使用公鑰解密，若訊息吻合則表示驗證成功

---

```
# 進入家目錄內的SSH目錄
$ cd ~/.ssh
```

```
# 產生SSH金鑰
$ ssh-keygen
```

```
# 使用RSA做為金鑰的加密演算法
$ ssh-keygen -t rsa
```

```
# 使用申請GitHub的電子郵件做為標籤
$ ssh-keygen -t rsa -C <email>
```

```
# 使用RSA做為金鑰的加密演算法，並指定金鑰長度為4096
$ ssh-keygen -t rsa -b 4096
```

```
# 讀取公鑰檔案內容
$ cat ~/.ssh/id_rsa.pub
```

```
# 複製金鑰檔案內容到剪貼簿
$ clip < ~/.ssh/id_rsa.pub
```

```
# 驗證GitHub的SSH綁定
$ ssh git@github.com
```

```
# 測試SSH，驗證GitHub的SSH綁定
$ ssh -T git@github.com
```