---
title: "程式初探系列 - Day 01 變數的宣告"
categories:
- 程式初探系列
- Javascript
tags:
- 程式初探
- javascript
- 變數宣告
date: 2022-11-06T21:24:33+08:00
draft: false
---

# 前言

本系列將以Javascript為例進行介紹，期望能讓更多人從0開始學習寫程式，並體會寫程式的樂趣。

# Javascript 基本介紹

JavaScript 屬於弱型別程式語言。這代表在撰寫程式碼時不必特別宣告變數的型別。程式在運作時，型別會自動轉換。

*註:相對於弱型別程式語言，強型別程式語言則會需要將每個變數定義好型別，否則會產生錯誤。程式在運作時，型別不會自動轉換。Java正屬於這種強型別程式語言。*

~~會心一笑:JavaScript之於Java就像狗之於熱狗，2者是完全不一樣的程式語言。~~

# Javascript 變數

在JavaScript的世界中，宣告變數的方法共有3種，分別是```var```、```let```、```const```。

# 變數宣告 var

Javascript在2015年以前的變數宣告方法只有```var```，且可以重複宣告。因此，如果要在舊版本瀏覽器運行程式碼。則需要使用```var```來進行變數宣告

## 舉例

{{< tabbed-codeblock var.js >}}
<!-- tab js -->
var x = 20                       // 宣告1個變數 x，其值為20
x = 10                           // 將宣告的變數 x 變更其值，成為10
var x = 30                       // 重新宣告變數 x，其值為10
<!-- endtab -->
{{< /tabbed-codeblock >}}


# 變數宣告 let

Javascript在2015年以後新增的變數宣告方法```let```，且**不可**重複宣告。

## 舉例

{{< tabbed-codeblock let.js >}}
<!-- tab js -->
let x = 20                       // 宣告1個變數 x，其值為20
x = 10                           // 將宣告的變數 x 變更其值，成為10
// let x = 30                    // **錯誤:不可重新宣告變數 x** 
<!-- endtab -->
{{< /tabbed-codeblock >}}

# 變數宣告 const

如果該變數不會變更，則應視為常數，以const進行宣告，且**不可**重複宣告。

## 舉例

{{< tabbed-codeblock const.js >}}
<!-- tab js -->
const x = 20                      // 宣告1個常數 x，其值為20
// x = 10                         // **錯誤:常數 x 不可變更其值**
// const x = 30                   // **錯誤:不可重新宣告變數 x ***
<!-- endtab -->
{{< /tabbed-codeblock >}}

# 小結

本篇介紹了Javascript中變數的宣告，不同的程式語言會有不同的宣告方式。

# 參考連結

* [w3schools - Variables](https://www.w3schools.com/js/js_variables.asp)
* [MDN Web Docs - Statements](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements)

