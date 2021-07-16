要點整理
- SHA-1 (Secure Hash Algorithm 1)，是==單向Hash雜湊加密演算法==，雜湊值由40個十六進位數字元組成
- ==碰撞==是指不一樣的輸入/檔案內容，卻有一樣的輸出/SHA-1值，發生碰撞的機率超低

---

```
# 檢視master的SHA-1雜湊值
$ cat .git/refs/heads/master
```