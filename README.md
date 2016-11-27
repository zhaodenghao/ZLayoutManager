# FlowLayoutManager
利用自定义LayoutManager 实现的流式布局。

## 相关博文
http://blog.csdn.net/zxt0601/article/details/52956504

我想说，如果需求是每个Item宽高一样，实现起来复杂度比每个Item宽高不一样的，要小10+倍。

然而我们今天要实现的流式布局，恰巧就是至少每个Item的宽度不一样，所以在计算坐标的时候算的我死去活来。先看一下效果图：

![这里写图片描述](https://github.com/mcxtzhang/FlowLayoutManager/blob/master/gifs/gif1)

艾玛，换成妹子图后貌似好看了许多，我都不认识它了，好吧，项目里它一般长下面这样：

![这里写图片描述](https://github.com/mcxtzhang/FlowLayoutManager/blob/master/gifs/gif2)

往常这种效果，我们一般使用自定义ViewGroup实现，我以前也写了一个。[自定义VG实现流式布局](http://blog.csdn.net/zxt0601/article/details/50533658)

这不最近再研究自定义LayoutManager么，想来想去也没有好的创意，就先拿它开第一刀吧。
（后话：流式布局Item宽度不一，不知不觉给自己挖了个大坑，造成拓展一些功能难度倍增，
观之网上的DEMO，99%Item的大小都是一样的
，so，这个系列的下一篇我计划 实现一个Item大小一样 的酷炫LayoutManager。
但是最终做成啥样的效果还没想好，有朋友看到酷炫的效果可以告诉我，我去高仿一个。）

