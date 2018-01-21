# Data-Visualization

1.概要
在看到泰坦尼克号数据集的时候，就回想起电影中船长“让妇女和儿童先上”的救生口号，然后就想统计下是否真的如电影所说。
	1）第一步先统计了不同人群的生还率发现真的妇女和儿童的生还率要高于男人的。
	2）但是在探究船舱等级的时候，发现头等舱的生还率明显高于其他两船舱。
	3）对比不同船舱等级的不同人群的生还比例，发现头等舱的不同人群生还几率都远高于其他两舱。
	4）做出强烈对比图（头等舱的妇女生还几率跟三等舱的男人生还几率对比图）来突出结论：在泰坦尼克号上执行口号这样表述可能更准确一些：‘头等舱和二等舱的妇女和儿童优先’。

2.设计
在初次可视化的时候，通过对比bar chart、area chart、bubble chart发现还是bar chart最能简单明了的突出主题，所以决定使用bar chart来设计最终的可视化。

为了能够让可视化的图显得更加简洁和平滑，我用python对titanic.csv进行的修改了。同时由于我对于d3的数据过滤不是很熟练，所以我使用python过滤出每个图所需要的不同数据保存到不同的csv文件中（例如：titanic_clean.csv等）。

3.反馈
1）反馈1：在设计过程中，曾经设计了不同年龄的生还几率，但是由于数据集的量不是很大，有的年龄人数很少，导致整个图看起来非常奇怪，十分不平滑。
处理结果：删除了此图，用python修改数据集，改成了不同人群（12岁以下是儿童，50岁以下是成人，50岁以上是老人）。

2）由于时间原因，还没有分享给更多的人看，等下次提交的时候补上。

4.资源：
https://github.com/PMSI-AlignAlytics/dimple/wiki/dimple.chart#customClassList
https://github.com/d3/d3/blob/master/API.md
http://www.runoob.com/css3/css3-transitions.html
http://dimplejs.org/examples_index.html