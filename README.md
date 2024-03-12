# Test-2-ZPL

## 簡介

本專案為一個模仿出圖片上 ZPL 標籤的 ZPL 語法範例

## 執行方法

### 方法一：使用 Labelary 網頁 ZPL 渲染器

1. 開啟以下帶好參數連結：
https://labelary.com/viewer.html?density=6&quality=grayscale&width=4&height=6&units=inches&index=0&rotation=0&zpl=%5EXA%0A%5EFO50%2C50%5EGB525%2C370%2C3%5EFS%0A%5EFO50%2C50%5EGB525%2C240%2C3%5EFS%0A%5ECF0%2C47%0A%0A%5EFO100%2C90%5EFDABCDE-12345%5EFS%0A%5EFO100%2C160%5EFDabcde-12345%5EFS%0A%5EFO100%2C230%5EFDABCDE-12345-abcde%5EFS%0A%5EBY2.5%2C2%2C50%5EFO130%2C310%5EBC%5EFD12345678%5EFS%0A%5EXZ%0A

2. 即可查看 ZPL 標籤的渲染效果。

### 方法二：使用 Labelary 網頁 ZPL 編輯器

1. 開啟以下網址：

[https://labelary.com/viewer.html](https://labelary.com/viewer.html)

2. 將 `label.txt` 檔案內的語法複製到 ZPL 語法框。

3. 按下「Redraw」按鈕，即可查看 ZPL 標籤的渲染效果。

### 方法三：實際傳送至標籤機列印

1. 將 `label.zpl` 檔案傳送至標籤機。

2. 即可列印出 ZPL 標籤。


## 想法說明

### 1. 畫出主要外框
`^FO50,50^GB525,370,3^FS`

### 2. 畫第二個矩形作分區。 由於原圖上半部分文字整體偏靠下，所以我也讓整體稍微靠近下緣
`^FO50,50^GB525,240,3^FS`

### 3. 通過我的觀察，條形碼起於"ABCDE-12345-abcde"的"B"的中線，始於"d"的中線


