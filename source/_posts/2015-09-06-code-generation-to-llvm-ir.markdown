---
layout: post
title: "Code generation to LLVM IR"
date: 2015-09-06 10:57:51 +0800
comments: true
categories: 
---



process:

    AST --> LLVM IR


makefile:

```makefile
	clang++ -g lexer.cpp  `llvm-config --cxxflags --ldflags --system-libs --libs core mcjit native` -O3 -o lexer -rdynamic -v -fno-rtti

```
<!-- more -->
demo:

{% img left /images/demo_codegen.jpg 700 500 'image' 'images' %}

codegen.cpp:

{% include_code codegen.cpp %}

