---
title: Как подсветить одинаковые ячейки в google sheets
categories:
  - other
tags:
  - untagged
---

- выделили диапазон
- кликнули "формат"
- условное форматирование
- форматирование ячеек "Ваша формула"
- вставили формулу ```=AND(NOT(ISBLANK(A1)); COUNTIF($A$1:$F; "=" & A1) > 1)```
- магия


<!-- image
![GitHub Logo](/images/logo.png)
Format: ![Alt Text](url)
-->

<!-- Link
[GitHub](http://github.com)
--->

<!-- to-do list
- [x] this is a complete item
- [ ] this is an incomplete item
-->

<!-- Table

First Header | Second Header
------------ | -------------
Content cell 1 | Content cell 2
Content column 1 | Content column 2

-->