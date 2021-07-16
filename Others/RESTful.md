要點整理
- RESTful透過HTTP來表達==語義化的路由設計==
- RESTful的設計在強調從路由結構就能看出要對什麼資料，進行什麼操作

---

HTTP Method
* GET (讀取)
* POST (新增)
* PUT (修改全部)
* PATCH (修改局部)
* DELETE (刪除)

RESTful風格
* 新增使用者 `POST` `/user`
* 查詢所有使用者 `GET` `/users`
* 查詢指定使用者 `GET` `/user/1`
* 修改使用者 `PUT` `/user/1`
* 刪除使用者 `DELETE` `/user/1`

RESTful風格
* 新增一篇文章 `POST` `/posts`
* 瀏覽全部文章 `GET` `/posts`
* 瀏覽一篇文章 `GET` `/posts/:id`
* 修改一篇文章 `PATCH` `/posts/:id`
* 刪除一篇文章 `DELETE` `/posts/:id`

傳統風格
* 新增使用者 `POST` `/user/new`
* 查詢所有使用者 `GET` `/users/all`
* 查詢指定使用者 `GET` `/user/query/1`
* 修改使用者 `PUT` `/user/update/1`
* 刪除使用者 `DELETE` `/user/delete/1`