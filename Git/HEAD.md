要點整理
- HEAD是一個指標，指向某個分支或版本，通常會指向當前分支，可以將HEAD當成目前所在分支
- HEAD不一定總會指向分支，當HEAD沒有指向分支的時候便會造成==斷頭== (detached HEAD)的狀態
- 分離HEAD是將HEAD指向某一個提交版本/commit，而不是某個分支
- ORIG_HEAD會存放HEAD的狀態，讓你在進行較危險的操作時，隨時可以跳回之前的狀態

---

```
# 檢視HEAD檔案的內容
$ cat .git/HEAD
```

```
# 查看HEAD指向的master分支內容
$ cat .git/refs/head/master
```

```
# 檢視ORIG_HEAD檔案的內容
$ cat .git/ORIG_HEAD
```