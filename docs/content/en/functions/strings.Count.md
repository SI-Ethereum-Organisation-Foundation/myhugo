---
title: strings.Count
description: Returns the number of non-overlapping instances of a substring within a string.
categories: [functions]
menu:
  docs:
    parent: functions
keywords: [count, counting, character count]
signature: ["strings.Count SUBSTR STRING"]
relatedfuncs: []
---

If `SUBSTR` is an empty string, this function returns 1 plus the number of Unicode code points in `STRING`.

Example|Result
:--|:--
`{{ "aaabaab" \| strings.Count "a" }}`|5
`{{ "aaabaab" \| strings.Count "aa" }}`|2
`{{ "aaabaab" \| strings.Count "aaa" }}`|1
`{{ "aaabaab" \| strings.Count "" }}`|8
