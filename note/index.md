# 笔记

## 前言

GIT学习推荐网站[《Pro Git（中文版）》](https://gitee.com/progit/)

## 1.安装

### 1.1 使用虚拟环境

虚拟环境工具`virtualenv`创建的一个虚拟环境，表现为一个文件夹，包含Python解释器和虚拟环境的各个包。
个人认为在操作系统环境相同的情况下，可复制虚拟环境文件夹直接使用。

### 1.2 使用pip安装Python包

pip 可以用-i参数指定pip源地址，如

```
pip install flask -i https://pypi.tuna.tsinghua.edu.cn/simple
```

## 2 程序的基本结构

### 2.1 初始化

* WSGI 协议
Python的web服务端程序可以分为两部分：web服务器(软件)和web项目。
其中web服务器负责将请求处理后转发给web项目，并将接收web项目的响应返回给客户端；web项目就是web开发的主要内容，根据不同的业务需求编写代码。
但是web服务器和web项目使用的框架种类都很多，在请求、响应参数传递过程中，如果没有同一的接口，会降低web服务器和web框架的通用性。
所以就有了WSGI协议。

WSGI协议：参考资料[PEP 3333](https://www.python.org/dev/peps/pep-3333/)。
该协议定义了统一的接口，任何符合该协议的web服务器和web框架都可以搭配使用。

* Flask程序实例

使用Flask框架开发的web项目就是一个Flask实例，代码中的各项配置，视图函数、路由、运行方式等代码都是以flask实例属性/方法的形式存在的。



