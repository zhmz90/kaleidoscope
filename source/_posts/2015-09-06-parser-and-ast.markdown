---
layout: post
title: "parser and AST"
date: 2015-09-06 10:57:37 +0800
comments: true
categories: 
---

AST type:
    
                             ExprAST 
                                
    NumberExprAST VariableExprAST BinaryExprAST CallExprAST FunctionAST PrototypeAST

Parsers:
            
    
    ParseExpression, ParseNumberExpr, ParsePrototype, ParseDefinition, ParseTopLevelExpr ...


makefile:

```makefile
	clang++ -g lexer.cpp  `llvm-config --cxxflags --ldflags --system-libs --libs core mcjit native` -O3 \
	-o lexer 
```
<!-- more-->

demo:

{% img left /images/demo_parser_ast.jpg 700 500 'image' 'images' %}

lexer_parser_ast code:

{% include_code parser_ast.cpp %}

