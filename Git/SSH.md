SSH連線運作方式
1. Client端發送SSH連線請求
2. Server端發送隨機訊息
3. Client端使用私鑰加密隨機訊息後並回傳加密訊息給Server端
4. Server端使用公鑰解密，若訊息吻合則表示驗證成功

要點整理
- 產生金鑰的過程會詢問3個問題，若沒有特殊需求可以全部使用預設值，按Enter留空即可
- 產生的金鑰有兩把，一把是新增到遠端倉庫/GitHub的公鑰，另一把是存放在本機的私鑰
- 設定金鑰代理是給有設定金鑰密碼的人，在每次使用金鑰時不需再輸入密碼

---

```
$ cd ~/.ssh									// 進入SSH目錄
```

```
$ ssh-keygen								// 產生SSH金鑰
```

```
$ ssh-keygen -t rsa							// 使用RSA做為金鑰的加密演算法
```

```
$ ssh-keygen -t rsa -C "email@demo.com"		// 使用申請GitHub的電子郵件做為標籤
```

```
$ ssh-keygen -t rsa -b 4096					// 使用RSA做為金鑰的加密演算法，並指定金鑰長度為4096
```

```
$ cat ~/.ssh/id_rsa.pub						// 讀取公鑰檔案內容
```

```
 $ clip < ~/.ssh/id_rsa.pub					// 複製金鑰檔案內容到剪貼簿
```

```
$ ssh git@github.com						// 驗證GitHub的SSH綁定
```

```
 $ ssh -T git@github.com					// 驗證GitHub的SSH綁定
```