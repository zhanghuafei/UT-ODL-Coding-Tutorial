
## Code Style

ODL代码将[google-code-style](http://google.github.io/styleguide/javaguide.html)作为主要的代码规范，其中，Column limit：100调整为120。（见4.4节）    

额外的，可参考阿里的[alibaba-java-style-guide](ttps://yq.aliyun.com/download/2719，)，该文档涉及更广泛的主题。

若google-code-style和alibaba-java-style-guide发生冲突，则以google-code-style为准。

## 字符编码			
为统一团队开发环境，编码格式应设置为UTF-8，换行符统一为LF。

注意此处的设置仅对新建文件生效。

![](images/image001.jpg)

## Formatter
Eclipse提供快速格式化功能，并支持格式profile的灵活配置。为使格式化满足ODL的要求Code Style，应根据下图导入UT提供的profile文件。

![](images/image002.png)

Formatter包含两种使用方式，一是对选中代码的码的格式化，使用快捷键Ctrl+Shift+F完成。二是对整个项目的格式化（待补充）。
