RGB顏色表示法 - 整數值
```
.red{background-color: rgb(255,0,0);}				// 紅色
.green{background-color: rgb(0,255,0);}				// 綠色
.blue{background-color: rgb(0,0,255);}				// 藍色
.white{background-color: rgb(255,255,255);}			// 白色
.balck{background-color: rgb(0,0,0);}				// 黑色
```

RGB顏色表示法 - 百分比值
```
.red{background-color: rgb(100%,0%,0%);}			// 紅色
.green{background-color: rgb(0%,100%,0%);}			// 綠色
.blue{background-color: rgb(0%,0%,100%);}			// 藍色
.white{background-color: rgb(100%,100%,100%);}		// 白色
.black{background-color: rgb(0%,0%,0%);}			// 黑色
```

RGBA顏色表示法
```
.red{background-color: rgba(255,0,0,.3);}			// 帶30%不透明度的紅色
.green{background-color: rgba(0,255,0,.5);}			// 帶50%不透明度的綠色
.blue{background-color: rgba(0,0,255,.7);}			// 帶70%不透明度的藍色
.transparent{background-color: rgba(0,0,0,0);}		// 透明黑色
```

```
.red{background-color: rgba(100%,0%,0%,.3);}		// 帶30%不透明的紅色
.green{background-color: rgba(0%,100%,0%,.5);}		// 帶50%不透明的綠色
.blue{background-color: rgba(0%,0%,100%,.7);}		// 帶70%不透明的藍色
.transparent{background-color: rgba(%0,%0,%0,0);}	// 透明黑色
```

定義後備顏色
```
.red{
	background-color:rgb(255,0,0);			// 瀏覽器若不支援RGBA的替代降級方案
	background-color:rgba(255,0,0,0.6);
}
```