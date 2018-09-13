---
layout:     post
title:     ionic3中checkBox的使用
subtitle:   
date:       2018-09-12
author:     orchidtjj
header-img: img/post-bg-cook.jpg
catalog: true
tags:
    - ionic3
    - angular
---

## 前言

简单记录一下ionic3中常见的开发控件使用

## 效果

![](https://raw.githubusercontent.com/orchidTJJ/orchidtjj.github.io/dc25cc6f83528398e7025543cd9d11ed62d552b5/img/source/checkbox.gif)


## 代码	
	
html:
```
<ion-checkbox (ng-model)="isDisabled" (ionChange)="checkboxChange("></ion-checkbox><a>启用</a>
```

ts:
```
	isDisabled: boolean = false;

	checkboxChange() {
		this.isDisabled = !this.isDisabled;
		console.log(this.isDisabled);
		this.footagesList = [];
		this.requestMfwWorkingFacesList(true);
	}
```
