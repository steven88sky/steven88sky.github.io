---
title: "程式初探系列 - Day 02 資料型別"
categories:
- 程式初探系列
- Javascript
tags:
- 程式初探
- javascript
- 資料型別
date: 2022-11-06T21:24:33+08:00
draft: false
---

# Javascript 的資料型別 (基礎型別)

**除了物件(Object)以外的所有資料型別皆屬基礎型別**

| 型別名稱 | 例子 |
| :-- | :-- |
| 布林型別 (boolean) | ```true```、```false``` |
| 未定義型別 (undefined) | ```undefined``` |
| 數字型別 (number) | ```123```、```+Infinity```、```-Infinity```、```NaN``` (Not a Number) |
| 字串型別 (string) | ```'Hello world'```、```"Hello world"``` |

# Javascript 的資料型別 (物件 object)

| 物件類型 | 例子 |
| :-- | :-- |
| 陣列 (object - Array) | ```[]```、```[1, 2, 3]```、```new Array()``` |
| 物件 (object - Object) | ```{}```、```{1}```、```{ key: value }```、```new Object()``` |
| 空型別 (object - Null) | ```null``` |

# 小結

本篇介紹了Javascript中不同的資料型別，當然不同的程式語言會有一些不同的型別。但以初學者而言，先了解以上資料型別即可。

# 小測驗

請根據上述教學並想想看以下例子屬於何種型別

{{< tabbed-codeblock exercise.js >}}
<!-- tab js -->
true
37
'Hello'
new Object()
"false"
'3.14'
1.05
'true'
null
'[]'
NaN
"123"
new Date()
new Boolean(true)
Number(5)
'NaN'
new Number(1)
"undefined"
'new Object()'
"World!"
Math.PI
new String("test")
"{ id: 1 }"
Boolean(false)
Infinity
[1, 6, 8]
undefined
{ id: 1 }
<!-- endtab -->
{{< /tabbed-codeblock >}}

# 解答

{{< tabbed-codeblock exercise-answer.js >}}
<!-- tab js -->
true                                                              // boolean
37                                                                // number
'Hello'                                                           // string
new Object()                                                      // object
"false"                                                           // string
'3.14'                                                            // string
1.05                                                              // number
'true'                                                            // string
null                                                              // object
'[]'                                                              // string
NaN                                                               // number
"123"                                                             // string
new Date()                                                        // object
new Boolean(true)                                                 // object 請不要這樣寫
Number(5)                                                         // number
'NaN'                                                             // string
new Number(1)                                                     // object 請不要這樣寫
"undefined"                                                       // string
'new Object()'                                                    // string
"World!"                                                          // string
Math.PI                                                           // number
new String("test")                                                // object 請不要這樣寫
"{ id: 1 }"                                                       // string
Boolean(false)                                                    // boolean 請不要這樣寫
Infinity                                                          // number
[1, 6, 8]                                                         // object
undefined                                                         // undefined
{ id: 1 }                                                         // object
<!-- endtab -->
{{< /tabbed-codeblock >}}



# 參考連結

* [w3schools - Datatypes](https://www.w3schools.com/js/js_datatypes.asp)
* [MDN Web Docs - Datatypes](https://developer.mozilla.org/zh-TW/docs/Web/JavaScript/Data_structures)

