# stuOS

## 项目介绍

本项目参考rCore，为个人学习项目。

## 系统特性

批处理系统。

## 安装运行

* 工具安装请参考rCore文档，https://github.com/rcore-os/rCore-Tutorial-v3。

* 在项目根目录或者`os`目录下`make run`以运行本项目。

* 根目录下`make run-log`或者`make run FLAGS=--features\ LOG`开启一些调试信息的输出，后者也可以在`os`目录中使用。

## 工作进展

### 已完成

* [x] 基本开发

* [x] 系统调用安全性处理。

* [x] 根据make选项，实现DEBUG之下级别的内核信息是否输出的选择。

### 未完成

* [ ] **实现一个应用程序A，能打印调用栈。**
* [ ] **扩展内核，统计执行异常的程序的异常情况（主要是各种特权级涉及的异常），能够打印异常程序的出错的地址和指令等信息。**
* [ ] 扩展内核，实现新系统调用get_taskinfo，能显示当前task的id和task name，实现一个应用程序B，能访问get_taskinfo系统调用。
* [ ] 扩展内核，能够统计多个应用的执行过程中系统调用编号和访问此系统调用的次数。
* [ ] 扩展内核，能够统计每个应用执行后的完成时间。
* [ ] 实现一个应用程序C，用sleep系统调用睡眠5秒。
* [ ] *拓展更多系统调用。*
