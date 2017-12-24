---
layout: post
title: 在markdown文件中导入Latex公式的方法
tags: [TIPS]
---
<script type="text/javascript" src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=default"></script>
从[这里](http://blog.csdn.net/xiahouzuoxin/article/details/26478179)看到的方法，记录一下。

##使用MathJax引擎
在html或md文件中添加
{% highlight js %}
<script type="text/javascript" src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=default"></script>
{% endhighlight %}
然后就可以在文件中使用Tex公式了,$$公式$$表示行间公式，本来Tex中使用```\(公式\)```表示行内公式，但因为Markdown中```\```是转义字符，所以在Markdown中输入行内公式使用```\\(公式\\)```，如下代码：

		$$x=\frac{-b\pm\sqrt{b^2-4ac}}{2a}$$

		\\(x=\frac{-b\pm\sqrt{b^2-4ac}}{2a}\\)

分别显示行间公式:

$$x=\frac{-b\pm\sqrt{b^2-4ac}}{2a}$$

和行内公式:\\(x=\frac{-b\pm\sqrt{b^2-4ac}}{2a}\\)