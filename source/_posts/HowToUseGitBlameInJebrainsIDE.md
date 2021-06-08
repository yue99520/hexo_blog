---
title: 如何在 Jetbrains IDE 中使用 Git Blame 功能
author: Ernie Lee
date: 2021-06-08 18:07:06
categories:
- Jetbrains IDE
tags: 
- jetbrains 
- git 
- blame
- IDE
---
- 難度：簡單
- 介紹 Git Blame
- Jetbrains IDE 的 Git Blame 功能圖文教學
<!--more-->

---

## 前言
日前會知道有這個功能是因為朋友使用 vs code 時有裝類似的插件，分享給我後一開始以為是那個插件獨有的功能，後來得知 git 本來就有一個指令 `git blame` ，讓我開始研究在 Jetbarins 系列 IDE 中該不會也支援吧！



一查之後還真的讓我找到，而且發覺意外的簡單，不過在開始教學前，還是得科普一下 Git Blame 吧：

## Git Blame 是什麼？

常常在維護其他人寫的程式碼時，有時候我們會想看某一行 code 到底誰寫的，無論你想要好好請教一下程式碼的作者，或是在心裡問候一番，你都會很需要 Git Blame 這個功能，Git Blame 是 git 中原生就有的一個功能，它可以讓我們知道文件的**每一行**最後修改的**版本**和**作者**，但是若使用原生的指令，使用起來實在很麻煩，不一定每個人都喜歡純指令做每一件事。

- [git-blame 官方文件](https://git-scm.com/docs/git-blame/2.31.0)

## Jetbrains IDE 中的 Git Blame

- 以下就是開啟 Git Blame 後的結果，在 Editor 的左邊可以看到每一行程式碼是由誰提交，除了作者以外，**commit 時間**、**commit 版本雜湊**等等，其實都可以顯示。

![](14190380472915.jpg)

- 開啟方式很簡單，只需要在 **Editor 顯示行數 的地方 右鍵** > **Annotate with Git Blame**。

![](14190384156051.jpg)

- 我們可以透過再次點擊 **右鍵** > **View** 來選擇我們想要顯示的內容。
- 註：Colors 與 Names 可以調整 Highlight 與顯示姓名的設定。

![](14190386184800.png)

