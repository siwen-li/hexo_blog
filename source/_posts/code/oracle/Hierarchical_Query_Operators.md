---
title: 层次查询运算符
categories:
  - [学习, Oracle]
tags:
  - sql
  - oracle
---


## 层次查询运算符

仅在层次查询中才有效的运算符有两个, `PRIOR` 和 `CONNECT_BY_ROOT`。

## PRIOR

在层次查询中, `CONNECT BY` 条件中的一个表达式必须由 `PRIOR` 运算符修饰。如果 `CONNECT BY` 条件是复合的, 则只需要一个条件使用 `PRIOR` 运算符, 尽管可以有多个 `PRIOR` 条件。`PRIOR` 为层次查询中的当前行的父行立即计算后面的表达式。

???+ info 
    `PRIOR` 最常用于与等号运算符比较列值。(`PRIOR` 关键字可以在运算符的任一边。)`PRIOR` 会导致 Oracle 使用父行中的列值。除等号(=)之外的其他运算符在 `CONNECT BY` 子句中理论上也是可能的。但是, 这些其他运算符创建的条件可能会导致通过可能的组合进行无限循环。在这种情况下, Oracle 会在运行时检测到循环并返回错误。


## CONNECT_BY_ROOT

`CONNECT_BY_ROOT` 是仅在层次查询中才有效的一元运算符。当使用此运算符限定列时, Oracle 将使用根行的数据返回列值。


???+ warning 
    不能在 `START WITH` 条件或 `CONNECT BY` 条件中指定此运算符。