---
layout: wiki
category: wiki
subcategory: internet
title: Ultimate Short Custom Number Formatting
publication: Stack Overflow
link: https://stackoverflow.com/questions/69773823/ultimate-short-custom-number-formatting-k-m-b-t-etc-q-d-googol
date: 2024-12-26
---

"sadly, the internal formatting in google sheets is by default able to work with only 3 types of numbers:

* positive (1, 2, 5, 10, ...)
* negative (-3, -9, -7, ...)
* zero (0)

this can be tweaked to show custom formatting like thousands K, millions M and regular small numbers:

<code>[>999999]0.0,,"M";[>999]0.0,"K";0</code>

or only thousands K, millions M, billions B

<code>[<999950]0.0,"K";[<999950000]0.0,,"M";0.0,,,"B"</code>

or only negative thousands K, negative millions M, negative billions B

<code>[>-999950]0.0,"K";[>-999950000]0.0,,"M";0.0,,,"B"</code>

or only millions M, billions B, trillions T:

<code>[<999950000]0.0,,"M";[<999950000000]0.0,,,"B";0.0,,,,"T"</code>

or only numbers from negative million M to positive million M:

<code>[>=999950]0.0,,"M";[<=-999950]0.0,,"M";0.0,"K"</code>

but you always got only 3 slots you can use, meaning that you can't have trillions as the 4th type/slot. fyi, the 4th slot exists, but it's reserved for text."
