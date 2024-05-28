---
title: js筆記
date: 2024-05-23 15:32:22
tags: 
- js 
- 陣列
---

## 陣列寫法
```
let colors = ["red", "blue", "black"];

let ary = ["blue", true, 5];

let books = [5, 30, 400, 100];
```
### 讀取陣列資料，了解陣列長度
```
console.log(colors[0]);
```
### 陣列是從0開始，第一個=0
```
let myColor = colors[0];
```
### 讀取長度.length
```
console.log(colors.length);
```
### 寫入，中間沒寫會變成空資料，依然存在
```
let color = [];
color[0] = "blue";
color[3] = "red"
console.log(color);
```
### 在陣列最後塞入資料 .push
```
color.push('pink');
console.log(color);
```
###在陣列最前面塞入資料 .unshift
```
color.unshift("black");
```

### 刪除陣列資料
### 刪除最後一個 .pop
```
color.pop();
```
### 刪除第一個 .shift
```
color.shift();
```
### 刪除指定資料 (0,1) 0為起始位置, 1為幾筆資料，目前為從最前面刪除一筆
```
color.splice(1, 1);
```