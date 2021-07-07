RGB顏色表示法 - 整數值
```
# .red{background-color:rgb(255,0,0);}
# .green{background-color:rgb(0,255,0);}
# .blue{background-color:rgb(0,0,255);}
# .white{background-color:rgb(255,255,255);}
# .balck{background-color:rgb(0,0,0);}
```

RGB顏色表示法 - 百分比值
```
# .red{background-color:rgb(100%,0%,0%);}
# .green{background-color:rgb(0%,100%,0%);}
# .blue{background-color:rgb(0%,0%,100%);}
# .white{background-color:rgb(100%,100%,100%);}
# .black{background-color:rgb(0%,0%,0%);}
```

RGBA顏色表示法
```
# 帶30%不透明度的紅色
# .red{background-color:rgba(255,0,0,.3);}

# 帶50%不透明度的綠色
# .green{background-color:rgba(0,255,0,.5);}

# 帶70%不透明度的藍色
# .blue{background-color:rgba(0,0,255,.7);}

# 透明黑色
# .transparent{background-color:rgba(0,0,0,0);}
```

```
# 帶30%不透明的紅色
# .red{background-color:rgba(100%,0%,0%,.3);}

# 帶50%不透明的綠色
# .green{background-color:rgba(0%,100%,0%,.5);}

# 帶70%不透明的藍色
# .blue{background-color:rgba(0%,0%,100%,.7);}

# 透明黑色
# .transparent{background-color:rgba(%0,%0,%0,0);}
```

定義後備顏色
```
# 瀏覽器若不支援RGBA的替代降級方案
# .red{background-color:rgb(255,0,0);background-color:rgba(255,0,0,0.6);}
```