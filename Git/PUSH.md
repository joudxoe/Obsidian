要點整理
- 若線上版本的內容比本機版本還新，會有推不上去的情況，這時要先拉線上的版本回來更新再推一次

---

```
$ git push -u origin master
```

```
$ git push origin master
```

```
$ git push
```

```
$ git push origin master:master			// PUSH本地的master分支更新Server上的master分支
```

```
$ git push origin master:jane			// PUSH本地的master分支，並在Server上建立jane分支
```

```
$ git push --force						// 強制PUSH，會有覆蓋檔案內容的問題
```

```
$ git push -f							// 強制PUSH，會有覆蓋檔案內容的問題
```