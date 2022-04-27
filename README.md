# HtmlWebModify
前端修改HTML元素-Bootstrap+jQuery，可制作单页邮件网页等

此代码使用的 Bootstrap5.1 和 jQuery1.10 。
主要实现的是在前端修改HTML元素的内容和属性。

实现方式：
鼠标划到元素上，元素背景变灰，右上角弹出一个按钮；
点击右上角的修改按钮，弹出一个Bootstrap的模态窗口；
模态窗口里面的文本框读取并展示了元素的文本/属性等；
在文本框修改，然后点击保存，模态窗口自动关闭，页面的HTML文本/属性被新的覆盖。

举例：
比如：<p>我喜欢吃苹果。</p>。鼠标划到p标签，p标签背景变色同时右上角出现一个修改按钮，点击修改按钮，弹出一个窗口，窗口的文本框里面读取并展示了“我喜欢吃苹果。”
这个时候把文字修改成“我喜欢喝牛奶~”。然后点击保存。HTML页面的p标签就变成了<p>我喜欢喝牛奶~。</p>

应用：
对于没有编程经验的用户来说，可以点击即修改HTML网页。

拓展：
可以利用压缩包的js和css文件对建好的Bootstrap的网页进行改造，形成可在线编辑的网页。
改造步骤：
1. 引入js文件，引入css文件。
2. 将原来的Bootstrap网页的要修改的元素进行下面的三个处理：
	2.1 添加类：ymTextClass（要修改p元素等加此类）、ymAttrClass（要修改href等加此类）、ymImgClass（要修改图片地址等加此类）。
	2.2 添加id。（id必须要有，写入的时候会用到。id的值随便定义都没有影响。）
	2.3 在元素外部添加div框架。（div框架默认写个ymdiv类）
	改后一般如下：

经过上面两步，即可实现HTML页面点击按钮修改元素了。

![元素上的按钮](https://github.com/meetuyu/HtmlWebModify/blob/main/1.jpg)
![点击按钮弹出模态窗口](https://github.com/meetuyu/HtmlWebModify/blob/main/2.jpg)
![图片可以改src链接地址](https://github.com/meetuyu/HtmlWebModify/blob/main/3.jpg)
![标题也能改](https://github.com/meetuyu/HtmlWebModify/blob/main/4.jpg)
开发不易。纯个人博客。blog.wulin.space
