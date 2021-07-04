要點整理
- SVG (Scalable Vector Graphics - 可伸縮失量圖形/可縮放向量圖形)
- SVG是一種使用XML描述/定義二維向量圖形的圖像格式
- SVG可以在放大或改變圖像尺寸的情況下，不會造成圖像的品質損失

---

圖像標籤
- `<svg>` <small>定義使用svg的圖像繪製</small>

---

嵌入SVG圖形
```
<svg width="300" height="200">
	<text x="10" y="20">這是一段測試文字</text>
	<text x="10" y="20" dx="0" dy="20">這是一段測試文字</text>
	<line x1="50" y1="50" x2="250" y2="150" />
	<rect x="50" y="50" width="200" height="100" />
	<circle cx="150" cy="100" r="70">
	抱歉，您的瀏覽器不支援SVG
</svg>
```