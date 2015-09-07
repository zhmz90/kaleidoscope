---
layout: post
title: "JIT and Opitmizer Support"
date: 2015-09-06 10:58:16 +0800
comments: true
categories: 
---

process:

    Just-in-time compilation and optimization

makefile:

```makefile
    clang++ -g lexer.cpp  `llvm-config --cxxflags --ldflags --system-libs --libs core mcjit native` -O3 -o lexer -rdynamic -v -fno-rtti
```

<!-- more -->

demo:

{% img left /images/demo_jit_opt.jpg 800 500 'image' 'images' %}


jit_opt.cpp:

{% include_code jit_opt.cpp %}
	
