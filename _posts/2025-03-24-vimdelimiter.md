---
layout: post
title: Changing surrounding delimiters in VIM
date: 2025-03-24 12:41:00
description:
tags: vim sed substitute
categories: vim
featured: true
---

Vim is magic. I had tu change the surrounding delimiters of strings.

Basically, I had text like below and wanted to replace the backquote delimiter.

```
| 0x10 | LDAi | 2 | Charge la valeur de l'opérande dans le registre A `[A := operande]` |
| 0x14 | LDAd | 2 | Charge la valeur dans la RAM pointée par l'opérande dans le registre A. `[A := Mem[opérande]]` |
| 0x18 | - | - | - |
| 0x1c | STA | 2 | Sauvegarde en mémoire la valeur du registre A à l'adresse donnée par l'opérande. `[Mem[opérande] := A]` |
| 0x20 | LDBi | 2 | Charge la valeur de l'opérande dans le registre B `[B := operande]` |
| 0x24 | LDBd | 2 | Charge la valeur dans la RAM pointée par l'opérande dans le registre B. `[B := Mem[opérande]]` |
```

Every string like `\`[A := operande]\`` was to be replaced by `{++[A := operande]++}`.

To do so with, it is as easy as 1) visually selecting the lines where you want a
modification (Ctrl + V), and 2) press ":" followed by the magic recipe 

```
s/`\(.*\)`/{++\1++}/g
```

which stands for :

- s .... g : substitue globally in the grammar  s/src_pattern/dst_pattern/g
- the source pattern is a repetition of which ever character `.* ` we capture in
  a group by the surrounding \( and \); This source pattern is surrounded by the
source delimiter, hence the backquotes
- the target pattern is the new delimiters surrounding the group copy/pasted
  with the \1
