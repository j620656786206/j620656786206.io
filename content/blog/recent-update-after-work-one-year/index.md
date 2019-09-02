---
title:  工作一年後近況更新
date: "2019-09-03"
description: "趁著工作即將屆滿一年來記錄一下自己在這一年做了些什麼，及學了哪些東西。"
---

# 近況
趁著工作即將屆滿一年來記錄一下自己在這一年做了些什麼，及學了哪些東西。

### React Native
一開始應徵的職位雖然是前端工程師，不過並不知道自己會被分配到寫手機的APP。雖然有從udemy上學過react native的課程，不過課堂內所做過的side projects架構跟實際工作上碰到的專案架構差距滿大的。首先我們公司專案用到的navigation套件是 [`react-native-navigation`](https://github.com/wix/react-native-navigation), 不過我們專案裡有多加了一個設定檔去定義每個頁面中包含了哪些子頁面，每個頁面會定義著頁面名稱name，頁面種類type，以及所要導向的目標頁面target。

其次掌管狀態state的套件這部分倒是跟課程中學到的一樣，用了[`redux`](https://chentsulin.github.io/redux/)，資料用[`immutable`](https://immutable-js.github.io/immutable-js/)的形式儲存成`Map`或者是`List`，當資料有要做變動的時候去呼叫相對應的method去更新資料。

處理非同步跟打API的部分後來則是導入了[`redux-observable`](https://github.com/redux-observable/redux-observable)，因為是從`rxjs`衍伸出來的一個套件，所以功能相當的強大，提供了許多operators可以使用，很多實際應用場景都有配上用場，而且語法上我覺得也很簡單易懂。

後來因應新增加的功能，我則是自己使用了[`react-native-table-component`](https://github.com/Gil2015/react-native-table-component#readme)以及[`react-native-svg`](https://github.com/react-native-community/react-native-svg)處理表格與canvas。

前半年除了這些工具之外，自己在程式寫法上也改了很多地方，舉凡component的interface定義以及props跟state設計上也都學了不少。

### Backend
手機專案完成了之後我便轉到後端，目前也還是在學習的狀況。舉凡[`Nodejs`](https://nodejs.org/en/)，[`express`](https://expressjs.com/), [`MongoDB`](https://www.mongodb.com/)，資料庫，資料結構設計，API設計，cache和session，驗證和授權等等，後端有太多東西所以目前也還是只能慢慢一點一點慢慢摸索...
