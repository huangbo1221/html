# 内联标签iframe
## 什么是内联标签
iframe标签规定一个内联框架。一个内联框架被用来在当前 HTML 文档中嵌入另一个文档。
iframe一般用来包含别的页面，例如我们可以在我们自己的网站页面加载别人网站的内容。

代码如下：

![img.png](img.png)

显示效果如下：

![img_1.png](img_1.png)

可以看出来，A页面嵌入了B页面

当然，也可以嵌入其他的网页，代码如下：

![img_2.png](img_2.png)

显示效果如下：

![img_4.png](img_4.png)

百度的页面拒绝了连接？？？
分析：在网页按F12，看下具体的报错，如下：

![img_5.png](img_5.png)


'X-Frame-Options' = 'sameorigin'.
百度的Nginx设置了如上的配置，再看看语法，如下：

![img_6.png](img_6.png)

仅允许同域名的页面嵌套使用！！！

## a标签和iframe标签的联合使用
代码如下：

![img_7.png](img_7.png)

显示效果如下：

![img_8.png](img_8.png)

然后点击“点击跳转”，显示效果如下：

![img_9.png](img_9.png)

