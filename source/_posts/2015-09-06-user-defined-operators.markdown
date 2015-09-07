---
layout: post
title: "User-defined Operators"
date: 2015-09-06 10:58:43 +0800
comments: true
categories: 
---

process:

    user defined types

makefile:

```makefile
    clang++ -g user_defined_types.cpp  `llvm-config --cxxflags --ldflags --system-libs --libs core mcjit native` -O3 -o lexer -rdynamic -v -fno-rtti
```

<!-- more-->


user_defined_types.cpp

{% include_code user_defined_types.cpp %}

