---
title: "Linux_skill"
date: 2024-07-30T21:56:01+08:00
lastmod: 2024-07-30T21:56:01+08:00
draft: true
keywords: []
description: ""
tags: []
categories: []
author: ""

# You can also close(false) or open(true) something for this content.
# P.S. comment can only be closed
comment: false
toc: false
autoCollapseToc: false
postMetaInFooter: false
hiddenFromHomePage: false
# You can also define another contentCopyright. e.g. contentCopyright: "This is another copyright."
contentCopyright: false
reward: false
mathjax: false
mathjaxEnableSingleDollar: false
mathjaxEnableAutoNumber: false

# You unlisted posts you might want not want the header or footer to show
hideHeaderAndFooter: false

# You can enable or disable out-of-date content warning for individual post.
# Comment this out to use the global config.
#enableOutdatedInfoWarning: false

flowchartDiagrams:
  enable: false
  options: ""

sequenceDiagrams: 
  enable: false
  options: ""

---

<!--more-->

# linux skill

"ctrl l" vs clear
- "ctrl l" 可以回看之前命令的输出

在终端输入命令过长，误触快捷键撤销
```
~> bindkeys | grep undo
"^X^U undo
"^Xu undo
"^_" undo

 ```

在系统oom时，最后的安全重启

- "alt prtsc r e i s u b"
    - alt prtsc 一直按住 [参考](https://wiki.archlinux.org/title/Keyboard_shortcuts)

tmux 复用当前会话
```
tmux ls
tmux at -t 0
```

按住"win" 按住鼠标左键 --- 拖动窗口
; 按住"win" 按住鼠标右键 --- 改变窗口大小


man fonts-conf
- [配置fontconfig](https://catcat.cc/post/2021-03-07/)

chattr +i

直接上传系统日志，找大大求助。
```
journalctl -b 0 | curl -F "c=@-" "https://fars.ee"
```



