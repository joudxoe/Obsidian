要點整理
- HEAD是一個指標，指向某一個分支，通常會指向目前所在的分支，可以將HEAD當成目前所在分支
- HEAD不一定總會指向分支，當HEAD沒有指向某個分支的時候便會造成斷頭 (detached HEAD)的狀態
- ORIG_HEAD會存放HEAD的狀態，讓你在進行較危險的操作時，隨時可以跳回之前的狀態

---

```
$ cat .git/HEAD						// HEAD檔記錄著HEAD的內容
```

```
$ cat .git/refs/head/master			// 查看HEAD指向的master分支內容
```

```
$ cat .git/ORIG_HEAD
```