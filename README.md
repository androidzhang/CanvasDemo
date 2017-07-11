为了演示Android中各种drawXXX方法的时候，我做了一个App，通过单击相应的按钮绘制相应的图形，主界面如下所示： 

![](http://img.blog.csdn.net/20151108232126887)


![](http://img.blog.csdn.net/20151108232146680)




![](http://img.blog.csdn.net/20151108232200269)


![](http://img.blog.csdn.net/20151108232233534)


![](http://img.blog.csdn.net/20151109210355235)



![](http://img.blog.csdn.net/20151109213516268)



![](http://img.blog.csdn.net/20151109224701585)



![](http://img.blog.csdn.net/20151109225312358)


![](http://img.blog.csdn.net/20151109232945887)


![](http://img.blog.csdn.net/20151110130029221)



![](http://img.blog.csdn.net/20151110194420777)


![](http://img.blog.csdn.net/20151110220321796)



![](http://img.blog.csdn.net/20151110235113668)



## 总结 ##



Canvas通过drawXXX等一些列的绘图方法决定了要绘制的图形的外形，我们可以通过自由组合绘制出我们想要的效果。drawXXX方法中的坐标都是基于当前绘图坐标系的坐标，而非Canvas坐标系，默认情况下二者重合。通过调用translate、rotate、scale等方法可以对绘图坐标系进行变换。

画笔Paint控制着所绘制的图形的具体外观，Paint默认的字体大小为12px，在绘制文本时我们往往要考虑密度density设置合适的字体大小。画笔的默认颜色为黑色，默认的style为FILL，默认的cap为BUTT，默认的线宽为0，参见下图所示：


![](http://img.blog.csdn.net/20151111001906335)

在画面状的图形时，如果Paint的style是FILL，那么绘制的就是填充面；如果是STROKE，那么绘制的就是轮廓线。