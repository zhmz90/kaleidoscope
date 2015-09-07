---
layout: post
title: "Control flow"
date: 2015-09-06 10:58:24 +0800
comments: true
categories: 
---



process:
    
    if then else


makefile:
```makefile
    clang++ -g lexer.cpp  `llvm-config --cxxflags --ldflags --system-libs --libs core mcjit native` -O3 -o lexer -rdynamic -v -fno-rtti
```
<!-- more-->

demo:
{% img left /images/demo_if.jpg 800 500 'image' 'images' %}


if.cpp:
{% include_code if.cpp %}
