#WEB js exercise 在這次的練習，可以體驗 js 如何在文件上處理資料的輸入與輸出。請打開index.html 並編輯 js/js.js 以完成以下要求。

# Requirement
## 1.點選新增按鈕時，可顯示新的待辦事項在清單中
提示1. 將新增的 TODO 以字串存取

提示2. 用上一步驟的資料 創建 todoElement
* 必須要有以下結構
```js
<a href="#" class="list-group-item">TODO的敘述文字</a>
```
提示3. 將此 todoElement 顯示到 todoListEle 裡面。

___

## 2.點選待辦事項時，可顯示變色表示已完成；點選已完成項目，則變回未完成之底色
提示1. 在新增的 todoElement 上監聽 click 事件，觸發時請執行以下行為：
* 將對應的 `todoData` [完成與否] 值設定為完成狀態(true)

提示2. 更新被點擊的 todoElement 的 class
```js
//如果他的[完成與否]狀態為未完成，結構如下
<a href="#" class="list-group-item">TODO的敘述文字</a>
//如果他的[完成與否]狀態為完成，則結構如下
<a href="#" class="list-group-item list-group-item-success">TODO的敘述文字</a>
```

___

## 3.點選“全部標示已完成”按鈕時，所有待辦事項皆變色
* 利用 for loop

___

## ID與className說明
* 待辦事項輸入欄  ID："todo-input"
* 待辦事項新增鈕  ID："todo-submit"
* 待辦事項"清單"  ID："todo-todoList"
* 待辦事項"節點"  ID："list-group-item"
* 全部標示已完成鈕  className："todo-allDone"

___

## 會用到的API
```js
document.createElement()

// 拿到 input 得值
document.getElementById("<input element id>").value  

// HTMLElement 的 API
document.getElementById("<whatever you want>").className = string : String
document.getElementById("<whatever you want>").appendChild(Element)

// hyperlink element 的 API
document.getElementById("<anchor element id>").href // 設定超連結

// 新增監聽事件
element.addEventListener

// 取得觸發監聽器的事件節點
e.currentTarget

// array 新增子物件
[].length // 取得 Array 裡面物件的數量

// 拿取每一個物件
for 迴圈
```
