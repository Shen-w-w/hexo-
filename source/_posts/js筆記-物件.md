---
title: js筆記
date: 2024-05-23 15:32:22
tags: 
- js 
- 物件
---


## 物件
```
let home = {
    motherName: "Mary",
    fatherName: "Tom",
    dog: 3,
    isWakeup: false
};
```
## 讀取物件資料 物件.資料名稱
```
console.log(home.dog);
let tomDogs = (home.dog);
```
## 新增物件資料 物件.物件屬性名稱 = 物件屬性
```
let myHome = {};
myHome.motherName = "Mary";
myHome.dog = 2
```
## 修改物件屬性 不用let直接寫
```
myHome.motherName = "Jane";
myHome.dog += 1;
```
## 刪除物件屬性
```
delete myHome.dog;
```
## 另一種方法 定義後讀取該定義名稱  物件["屬姓名"] ->限字串
```
let a = myHome.motherName;
console.log(a);
console.log(myHome["motherName"]);
```
## jason小知識 屬姓名為數字時，只能透過物件["屬姓名"]選取
```
myHome["001"] = "hi";
```
## 陣列物件混合
```
let market = [
    {
        bossName: "Tom",
        bananaNum: 6,
        appleNum: 5
    },
    {
        bossName: "John",
        bananaNum: 9,
        appleNum: 8
    }
]
```
## 選取資料
```
console.log(market[0].bossName);
```
## jason :資料庫可讀取的共同格式

## 物件裡面還能包物件
```
let aHome = {
    motherStatus: {
        motherName: "mary",
        motherAge: 30
    },
    fatherStatus: {
        fatherName: "Ben",
        motherAge: 32
    },
    dogs: 3
}
```