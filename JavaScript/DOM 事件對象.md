要點整理
- 引起事件發生的動作稱為觸發事件

---

滑鼠事件對象
- `onclick` <small>單擊滑鼠左鍵時觸發事件</small>
- `oncontextmenu` <small>點擊滑鼠右鍵打開上下文菜單時觸發</small>
- `ondbclick` <small>雙擊滑鼠左鍵時觸發事件</small>
- `onmouseup` <small>按下滑鼠後鬆開時觸發事件</small>
- `onmousedown` <small>按下滑鼠時觸發事件</small>
- `onmouseenter` <small>當滑鼠移動到元素上時觸發，不支持冒泡</small>
- `onmouseleave` <small>當滑鼠移出元素時觸發</small>
- `onmouseover` <small>當游標移到對象範圍的上方時觸發事件</small>
- `onmousemove` <small>移動滑鼠時觸發事件</small>
- `onmouseout` <small>游標離開對象範圍時觸發事件</small>

鍵盤事件對象
- `onkeypress` <small>按下鍵盤字母數字鍵後鬆開觸發事件</small>
- `onkeydown` <small>按下鍵盤任何按鍵時觸發事件</small>
- `onkeyup` <small>按下鍵盤任何按鍵後鬆開觸發事件</small>

頁面事件對象
- `onabort` <small>圖片下載時被用戶中斷時觸發事件</small>
- `onbeforeunload` <small>在即將離開頁面 (刷新或關閉)時觸發</small>
- `onerror` <small>在加載圖像或文檔發生錯誤時觸發</small>
- `onhaschange` <small>當URL的錨點書籤發生修改時觸發</small>
- `onload` <small>頁面內容加載完成時觸發事件</small>
- `onpageshow` <small>在用戶訪問頁面時觸發</small>
- `onpagehide` <small>在用戶離開當前頁面跳轉到另一個頁面時觸發</small>
- `onresize` <small>瀏覽器窗口大小被改變時觸發事件</small>
- `onscroll` <small>當頁面被滾動時觸發事件</small>
- `onunload` <small>頁面將被改變時觸發事件</small>

表單事件對象
- `onblur` <small>當元素失去焦點時觸發事件</small>
- `onchange` <small>元素內容發生改變且失去焦點時觸發事件</small>
- `onfocus` <small>某個元素獲得焦點時觸發事件</small>
- `onfocusin` <small>元素即將獲取焦點時觸發事件</small>
- `onfocusout` <small>元素即將失去焦點時觸發事件</small>
- `oninput` <small>元素獲取用戶輸入時觸發事件</small>
- `onreset` <small>清除表單內容時觸發事件</small>
- `onsearch` <small>用戶於輸入文本搜索時觸發事件</small>
- `onselect` <small>選取文本時觸發事件</small>
- `onsubmit` <small>提交表單時觸發事件</small>

剪貼簿事件對象
- `oncopy` <small>拷貝元素內容時觸發</small>
- `oncut` <small>剪切元素內容時觸發</small>
- `onpaste` <small>貼上元素內容時觸發</small>

打印事件對象
- `onafterprint` <small>在頁面已經開始打印或打印窗口關閉時觸發</small>
- `onbeforeprint` <small>在頁面即將開始打印時觸發</small>

拖動事件對象
- `ondrag` <small>正在拖動元素時觸發</small>
- `ondragend` <small>拖動元素完成時觸發</small>
- `ondragenter` <small>拖動的元素進入放置目標時觸發</small>
- `ondragleave` <small>拖動的元素離開放置目標時觸發</small>
- `ondragover` <small>拖動的元素在放置目標上時觸發</small>
- `ondragstart` <small>在用戶開始拖動元素時觸發</small>
- `ondrop` <small>將拖動元素放置在目標區域時觸發</small>

多媒體事件對象
- `onabort` <small>在媒體終止加載時觸發</small>
- `oncanplay` <small>在可以開始播放媒體時觸發</small>
- `oncanplaythrough` <small>在可以正常播放媒體且無需停頓或緩衝時觸發</small>
- `ondurationchange` <small>在媒體的時長發生變化時觸發</small>
- `onemptied` <small>當播放列表為空時觸發</small>
- `onended` <small>在媒體播放結束時觸發</small>
- `onerror` <small>在媒體加載期間發生錯誤時觸發</small>
- `onloadeddata` <small>在瀏覽器加載媒體當前幀時觸發</small>
- `onloadedmetadata` <small>在媒體的元數據加載後觸發</small>
- `onloadstart` <small>在瀏覽器開始尋找指定媒體資源時觸發</small>
- `onpause` <small>在媒體暫停時觸發</small>
- `onplay` <small>在媒體開始播放時觸發</small>
- `onplaying` <small>在媒體暫停或緩衝後準備重新開始播放時觸發</small>
- `onprogress` <small>在瀏覽器下載指定的媒體時觸發</small>
- `onratechange` <small>在媒體的播放速率改變時觸發</small>
- `onseeked` <small>在用戶重新定位媒體的播放位置後觸發</small>
- `onseeking` <small>在用戶開始重新定位媒體時觸發</small>
- `onstalled` <small>在瀏覽器獲取媒體數據，但媒體數據不可用時觸發</small>
- `onsuspend` <small>在瀏覽器讀取媒體數據中止時觸發</small>
- `ontimeupdate` <small>在當前的播放位置改變時觸發</small>
- `onvolumechange` <small>在音量發生改變時觸發</small>
- `onwaiting` <small>在媒體要播放下一幀而需要緩衝時觸發</small>

動畫事件對象
- `animationend` <small>在CSS動畫結束播放時觸發</small>
- `animationiteration` <small>在CSS動畫重覆播放時觸發</small>
- `animationstart` <small>在CSS動畫開始播放時觸發</small>

過渡事件對象
- `transitionend` <small>在CSS完成過渡後觸發</small>

其它事件對象
- `onmessage` <small>通過從對象 (Websocket, Web Worker, Event Source…)接收到消息時觸發</small>
- `ononline` <small>在瀏覽器上線工作時觸發</small>
- `onoffline` <small>在瀏覽器離線工作時觸發</small>
- `onshow` <small>當menu元素在上下文菜單顯示時觸發</small>
- `onstorage` <small>在Web Storage更新時觸發</small>
- `ontoggle` <small>在用戶打開或關閉details元素時觸發</small>
- `onwheel` <small>滑鼠滾輪在元素上下滾動時觸發</small>

---

事件對象方法
- `initEvent()` <small>初始化新建的Event對象的屬性</small>
- `preventDefault()` <small>通知瀏覽器不要執行與事件關聯的默認動作</small>
- `stopPropagation()` <small>不再派發事件</small>

目標事件對象方法
- `addEventListener()` <small>在目標事件中註冊監聽事件</small>
- `dispatchEvent()` <small>允許發送事件到監聽器上</small>
- `removeEventListener()` <small>移除註冊在目標事件上的監聽事件</small>

事件監聽對象方法
- `handleEvent()` <small>將任意對象註冊為事件處理程序</small>

---

事件對象屬性
- `bubbles` <small>返回事件是否為起泡事件類型</small>
- `cancelable` <small>返回事件是否可取消默認的動作</small>
- `currentTarget` <small>返回觸發事件監聽器的元素</small>
- `eventPhase` <small>返回事件傳播的當前階段</small>
- `target` <small>返回觸發此事件的元素</small>
- `timeStamp` <small>返回事件生成的日期和時間</small>
- `type` <small>返回當前事件對象表示的事件名稱</small>

滑鼠/鍵盤事件對象屬性
- `altKey` <small>返回事件被觸發時，ALT鍵是否被按下</small>
- `button` <small>返回事件被觸發時，被點擊的滑鼠按鈕</small>
- `clientX` <small>返回事件被觸發時，游標的水平座標</small>
- `clientY` <small>返回事件被觸發時，游標的垂直座標</small>
- `ctrlKey` <small>返回事件被觸發時，CTRL鍵是否被按下</small>
- `Location` <small>返回按鍵在設備上的位置</small>
- `charCode` <small>返回onkeypress事件觸發鍵值的字母代碼</small>
- `key` <small>返回按下按鍵的標示符</small>
- `keyCode` <small>返回onkeypress事件觸發鍵值的字符代碼</small>
- `which` <small>返回onkeypress事件觸發鍵值的字符代碼</small>
- `metaKey` <small>返回事件被觸發時，meta鍵是否被按下</small>
- `relatedTarget` <small>返回與目標事件相關的節點</small>
- `screenX` <small>返回事件被觸發時，游標的水平座標</small>
- `screenY` <small>返回事件被觸發時，游標的垂直座標</small>
- `shiftKey` <small>返回事件被觸發時，SHIFT鍵是否被按下</small>