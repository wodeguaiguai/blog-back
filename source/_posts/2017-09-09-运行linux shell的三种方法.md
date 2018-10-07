---
layout: post
title:  "运行linux shell的三种方法"
categories: 
- tips
tags:  
- linux
- shell
author: 我的乖乖
---

1. 使文件具有可执行权限，直接运行文件
2. 直接调用命令解释器执行程序
3. 使用source执行文件
 > - 使用source执行shell脚本时，不会创建子进程，而是在父进程中直接执行！ 
 - 和其他运行脚本不通，source命令影响shell进程本身。在脚本的执行过程中，并没有进程创建和消亡。
 - 当需要在程序中修改当前shell本身的环境变量时，使用souorce命令。