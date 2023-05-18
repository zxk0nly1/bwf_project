# 课程安排 

第一天：appium介绍(工作原理，特点)，搭建appium环境，appium元素定位(5种)， 

appium元素操作(常用api) 

第二天：pytest(单元测试框架，作用同unittest，但是是第三方的)，PO模型(最难)

## 1.回顾 

### 什么是自动化测试？

```
   编写自动化代码(脚本)，让计算机执行代码，代替手工执行测试的过程。自动化测试的步骤/思
路与手工测试是一样的。
```

## 自动化测试分类： 

#### UI 自动化测试 

web UI自动化 ==》selenium 

app UI自动化 ==》appium 

#### 接口自动化测试 

requests ===》纯写代码 

jmeter+ant+jenkins ====》带界面工具 

##### 自动化测试好处：帮助做回归测试，提高效率，避免人为错误等 

##### 自动化测试时间：一般是在功能测试基本完成，版本比较稳定，没有大问题，时间比较充裕， 就可以开展自动化测试

#### 自动化测试流程： 

```
1）评估自动化测试可行性（考虑因素：项目周期，版本比较稳定，项目需要迭代，需求变更不
频繁等）
2）分析需求，制定自动化测试计划（测试范围，工具，编程语言，测试框架，人员安排，时
间安排等）
测试范围：主业务流程，主功能，频繁使用功能，容易出错的功能等
3）准备手工测试的测试用例（直接从手工测试用例中抽取符合要求用例，方便自动化测试用
例编写时可以参考）
4）搭建自动化测试的环境和框架。
python+selenium+unittest+HTMLTestRunner+PO(UI自动化设计模式，
base/case/report/page/data)+jenkins(持续集成===自动化项目可以自动周期性执行)
5）根据自动化测试计划，编写自动化代码。
6）将代码上传代码服务器(svn，git等)，批量执行，生成测试报告。
7）集成jenkins工具，实现自动化项目持续集成，可以实现无人值守，日常巡检。
```



## 2.appium介绍 

appium是一款开源自动化测试工具，可以支持多语言（python，java等），支持跨平台 

(windows,linux,macos)，支持android和ios平台的APP应用。其实appium是对selenium 

的一个扩展，很多方法的使用与selenium类似。

### 3.appium运行原理 

![1684416028781](C:\Users\12726\AppData\Local\Temp\1684416028781.png)

### 4.appium环境搭建 

##### 1.jdk安装以及环境配置 

验证：在cmd输入命令：java -version 

##### 2.sdk安装以及环境配置 

验证：在cmd输入命令：adb

##### 3.逍遥模拟器 

##### 4.python环境 

* python编译器 
* python开发环境==pycharm 

##### 5.安装node.js 

原因：appium是用node.js开发的。 

验证：在cmd输入命令：node -v 

##### 6.安装appium客户端 

打开cmd，输入命令：pip install Appium-Python-Client==1.0.2 

验证：在cmd，输入命令：pip list 

##### 7.安装appium服务端 

安装appium-installer.exe



