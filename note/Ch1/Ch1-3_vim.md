# Chapter 1 - 3_Intro to Vim

###### tags: `Python Troj` `Chapter 1`

 - Intro to Vim
     - [Installation](#Installation)
         - [CLI](#CLI)
         - [Visual Studio Code](#VSCode)
     - [Basics](#Basics)
         - [Insert / Save](#Insert--Save)
         - [Copy / Paste](#Copy--Paste)
         - [Undo / Redo](#Undo--Redo)
         - [Find / Delete / Substitute](#Find--Delete--Substitute)
         - [Indentation](#Indentation)
         - [Comment](#Comment)
     - [Additional](#Additional)
         - [Multi-line Append](#Multi-line-Append)
         - [Bulk Removal](#Bulk-Removal)
 - Appendix
     - [Modes](#Modes)
         - [Normal  Mode](#Normal-Mode)
         - [Insert  Mode](#Insert-Mode)
         - [Visual  Mode](#Visual-Mode)
         - [Command Mode](#Command-Mode)
    - [Resources](#Resources)

## 學習目標
:::info
學會用 vim 來當作打程式的工具
熟記基礎的指令，認識進階的技巧
:::
<!--
小練習
1. 一口氣貼上10次剛剛複製的東西
:::spoiler 答案
10p
:::

3. 把"www"全部換成"mmm"
:::spoiler
:%s/www/mmm/g
:::
5. 把排版修好
:::spoiler
gg=G
:::
7. 刪掉第4-8行
:::spoiler
:4,8d
:::
9. 刪掉\`\`之間的東西
:::spoiler
ca\`
:::
11. 跳到行尾並進入insert mode
:::spoiler
A
:::
-->

## **Installation**

### CLI

`$ sudo apt install vim`

### VSCode

![](https://hackmd.io/_uploads/S1VwCjGM3.png)

## **Basics**

### Insert / Save
:::info
`i` : insert to current position
:::
![](https://hackmd.io/_uploads/r1Liv2zM2.gif)
:::info
`o` : insert to next line
:::
![](https://hackmd.io/_uploads/HJh2qnzGh.gif)
:::info
`A` : Append to current line
:::
![](https://hackmd.io/_uploads/S1BJC2fzh.gif)

### Copy / Paste
:::info
`yy` : copy current line
:::
:::info
`p` : paste 
:::
![](https://hackmd.io/_uploads/Byg-Gazf2.gif)

### Undo / Redo
:::info
`u` : undo
:::
:::info
`ctrl + r` : redo
:::
![](https://hackmd.io/_uploads/r1qJ03fz3.gif)

### Find / Delete / Substitute
:::info
`/<pattern>` : find the pattern
:::
![](https://hackmd.io/_uploads/rkylA3fMh.gif)

:::info
`x` : delete the character under the cursor
:::
![](https://hackmd.io/_uploads/S11hAhGM2.gif)

:::info
`dd` : delete the entire line
:::
![](https://hackmd.io/_uploads/S196RhzG2.gif)

:::info
`:%d` : delete the entire file
:::
![](https://hackmd.io/_uploads/B1teGazGn.gif)

:::info
`s` : delete and insert
:::
![](https://hackmd.io/_uploads/ryPgMaMM2.gif)

:::info
`:%s/<pattern1>/<pattern2>/g` : replace pattern1 with pattern2, all occurrences
:::
![](https://hackmd.io/_uploads/SyrefaMGn.gif)

:::info
`:2,10s/<pattern1>/<pattern2>/g` : replace pattern1 with pattern2 from line 2 to 10
:::
![](https://hackmd.io/_uploads/HkzgzpGz2.gif)

### Indentation
:::info
`>>` : right shift tab width
:::

:::info
`<<` : left shift tab width
:::

:::info
`=` : fix the indentation
:::
![](https://hackmd.io/_uploads/r13awpfGh.gif)


:::success
`gg=G` : fix the indentation from the start to the end of the file
:::
![](https://hackmd.io/_uploads/SyRTwTMG2.gif)

### Comment

:::info
`gcc` : comment out the current line
:::

## **Additional**

### Multi-line Append

:::success
`:2,10s/$/word/`
:::
![](https://hackmd.io/_uploads/HyNAP6Mfn.gif)

:::success
`vip<C-V>$A<word><Esc>`
:::
![](https://hackmd.io/_uploads/Sy-yuafGh.gif)

### Bulk Removal

:::success
`caw` : remove a single word
:::
![](https://hackmd.io/_uploads/rkebq6zG2.gif)

:::success
`ca"` : remove the sentence inside the double quote    
:::
![](https://hackmd.io/_uploads/HyfW5azf3.gif)

:::success
`ca[` : remove everything inside the brackets
:::
![](https://hackmd.io/_uploads/H1m-cTGf3.gif)


---

## **Modes**

![](https://hackmd.io/_uploads/ByrDcTMzh.png)

    
### Normal Mode

idle state

press `esc` to return to normal mode in any other mode

### Insert Mode

works like a normal editor

### Visual Mode

press `v` to select words

### Command Mode

press `:` to pass commands

## **Resources**

### Interactive Page
[Interactive Vim Tutorial](https://www.openvim.com/)

### Text Guide
[Learn-Vim](https://github.com/iggredible/Learn-Vim)

### Videos
[Mastering the Vim Language](https://www.youtube.com/watch?v=wlR5gYd6um0)
[How to Do 90% of What Plugins Do (With Just Vim)](https://www.youtube.com/watch?v=XA2WjJbmmoM)