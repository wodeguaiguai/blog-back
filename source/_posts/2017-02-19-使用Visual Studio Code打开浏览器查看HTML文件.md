---
layout: post
title:  "使用Visual Studio Code打开浏览器查看HTML文件"
categories: tips
tags:  tips vscode
author: 我的乖乖
---


 1. 首先界面按下Ctrl+Shift+P显示命令面板，输入ctr
 2. 然后选择【Others】，可以看到默认配置
 3. 最后修改如下(删除其中一行)：
 ```json
    {
        "version": "0.1.0",
        "command": "Chrome",
        "windows": {
            "command": "C:/Program Files (x86)/Google/Chrome/Application/chrome.exe"
        },
        "args": ["${file}"],
        "showOutput": "never"
    }
 ```
 4. 快捷键Ctrl+Shift+B打开浏览器查看该文件，快捷键Ctrl+Shift+V来预览该html文件