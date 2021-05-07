要點整理
- XML (eXtensible Markup Language - 可擴展標記/標識語言/可延伸標籤語言)
- XML是一種==必須正確標記==且格式良好的標記語言
- XML不是HTML的替代，XML主要用於傳輸和儲存數據，HTML用於格式化並顯示數據
- XML設計用於傳輸資料，而不是顯示資料
- XML沒有預定義標籤，需要使用者自定義所需的標籤(tags)
- XML著重於如何將文件資料用==結構化格式==來表示
- 合法的XML文檔遵守==文檔類型定義==(DTD)的語法規則
- XML命名空間在元素前增加一個前綴來保證元素和屬性的唯一性，可融合不同的XML文檔

XML規範
- XML元素都必須有==關閉標籤==
- XML標籤對==大小寫敏感==
- XML元素必須==正確的嵌套==
- XML文檔必須有==根元素==，也就是有一個元素是所有其它元素的父元素
- XML的屬性值需加==引號==
- 在XML中，特殊字符必須使用==實體引用==
- 在XML的多個連續空格會被保留，不會被刪除/裁減成一個

XML文檔結構
```
<?xml version="1.0" encoding="utf-8"?>	<!-XML文件宣告/文檔聲明-->
<bookstore>
	<book category="COOKING">
	  <title lang="en">Everyday Italian</title> 
	  <author>Giada De Laurentiis</author> 
	  <year>2005</year> 
	  <price>30.00</price> 
	</book>
	<book category="CHILDREN">
	  <title lang="en">Harry Potter</title> 
	  <author>J K. Rowling</author> 
	  <year>2005</year> 
	  <price>29.99</price> 
	</book>
	<book category="WEB">
	  <title lang="en">Learning XML</title> 
	  <author>Erik T. Ray</author> 
	  <year>2003</year> 
	  <price>39.95</price> 
	</book>
</bookstore>
```