
# Code Style

ODL代码将[google-code-style](http://google.github.io/styleguide/javaguide.html)作为主要的代码规范，其中，Column limit：100调整为120。（见4.4节）    

额外的，可参考阿里的[alibaba-java-style-guide](ttps://yq.aliyun.com/download/2719，)，该文档涉及更广泛的主题。

若google-code-style和alibaba-java-style-guide发生冲突，则以google-code-style为准。

#Environment
## Eclipse初始配置
[GettingStarted:_Eclipse](https://wiki.opendaylight.org/view/GettingStarted:_Eclipse)
## 字符编码			
为统一团队开发环境，编码格式应设置为UTF-8，换行符统一为LF。

注意此处的设置仅对新建文件生效。

![](images/image001.jpg)

## Formatter
Eclipse提供快速格式化功能，并支持格式profile的灵活配置。为使格式化满足ODL的要求Code Style，应根据下图导入UT提供的profile文件。

![](images/image002.png)

Formatter包含两种使用方式，一是对选中代码的码的格式化，使用快捷键Ctrl+Shift+F完成。二是对整个项目的格式化（待补充）。

## CheckStyle
### Step 1- Install Check-Style Plugin
- 方法1：通过Eclipse市场安装    
进入菜单Help -> Eclipse Market Place -> Search  
    搜索checkstyle
- 方法2：    
Help-> Install New Software  
    CheckStyle插件地址：http://eclipse-cs.sourceforge.net/update  
    安装完成后，根据提示重启eclipse即安装完成。

### Step 2- Check Configuration
按图导入如下三个check configuration文件并设为默认配置：
- [odl_checks.xml](https://github.com/zhanghuafei/ODL-Coding-Guidelines/blob/master/check-style/odl_checks.xml)
- [checkstyle-suppressions.xml](https://github.com/zhanghuafei/ODL-Coding-Guidelines/blob/master/check-style/checkstyle-suppressions.xml)
- [EPL-LICENSE.regexp.txt](https://github.com/zhanghuafei/ODL-Coding-Guidelines/blob/master/check-style/EPL-LICENSE.regexp.txt)

进入菜单Windows -> Preferences -> Check Style
![](images/image004.png)

### Step 3- Activate checkstyle
![](images/image005.jpg)

### Step 4 - Make Sure whether ChecStyle take effect
![](images/image006.png)

## 添加版权声明

通过如图的设置，可在新建文件时，自动将如下版权声明添加到文件中：
```
/*
 * Copyright (c) 2018 UTStarcom, Inc. and others. All rights reserved.
 *
 * This program and the accompanying materials are made available under the
 * terms of the Eclipse Public License v1.0 which accompanies this distribution,
 * and is available at http://www.eclipse.org/legal/epl-v10.html
 */
```

![](images/image007.png)

## Organize Imports
去掉Eclipse所有预置的import order。

![](images/image008.jpg)

## Save Actions (Optional)
该设置可在保存文件时触发图中指定的动作，因勾选该项将导致保存文件速度过慢，所以请按需设置。

![](images/image009.jpg)

## 2.8.	代码自动提示功能

![](images/image010.jpg)

