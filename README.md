# KeyPointView
一个获取路径关键点的算法

假设我们绘制一条曲线，但是这条曲线可能就是一条折现，那么构成这条折现的组成关键点就只需要3个点就可以.



![image](https://raw.githubusercontent.com/jimmyleeking/KeyPointView/master/demoShow.gif)
原本想要用Ramer–Douglas–Peucker这个通常意义上的压缩算法来实现，但是后来发现如果这个算法不改进的话，
会存在一个严重的问题：起始点和终点一，只能得到起点和终点。

通过简单的三角函数+归并算法，来对路径的特征关键点进行提取。
具体效果如下：

