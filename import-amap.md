# 从高德云图导入数据

地图无忧支持导入第三方的地图数据，高德云图是其中之一。本文介绍一下，如何导入高德云图的数据。

首先，你得从高德云图把数据导出来。进入高德云图的地图管理页面，如图所示，点击地图名旁边的**小箭头**，再选择**导出数据**，数据就被下载为CSV文件了。

![](http://pic.dituwuyou.com/map%2Fpicture%2F%E4%BB%8E%E9%AB%98%E5%BE%B7%E4%BA%91%E5%9B%BE%E5%AF%BC%E5%85%A5%E6%95%B0%E6%8D%AE1.png)

下载下来的文件，可以打开看一下，做些简单的修改，比如把**其中的id列删除**或重命名为序号（id为程序关键字，不建议使用），createtime和updatetime这些列也可以删除，一般没什么作用。

然后按照上传文件的方式，批量上传到地图无忧即可，具体如下三步。

1：登录地图无忧网站，「**进入工作台**」后，点击「**新建地图**」 ，进入地图编辑页面。

2：在左侧数据操作列表中，点击「**批量添加数据**」 ；在弹出的对话框中默认的「本地上传 」页面 ，点击「**选择数据**」，选择刚才下载的文件进行上传。

【注意，如果提示文件解析错误，那是因为在部分Windows电脑下从高德云图导出的CSV格式为ANSI编码，需要先将转换为UTF8编码（比如用nodepad++等工具），然后再重新上传即可。】

![](http://pic.dituwuyou.com/map%2Fpicture%2F%E4%BB%8E%E9%AB%98%E5%BE%B7%E4%BA%91%E5%9B%BE%E5%AF%BC%E5%85%A5%E6%95%B0%E6%8D%AE2.png)

3：在新弹出的对话框中，选择标题，以及对应的**经度列、纬度列**，并特别注意选择**Google/高德坐标系**，让添加的标注点位置能够正确显示在地图上。
![](http://pic.dituwuyou.com/map%2Fpicture%2F%E4%BB%8E%E9%AB%98%E5%BE%B7%E4%BA%91%E5%9B%BE%E5%AF%BC%E5%85%A5%E6%95%B0%E6%8D%AE3.png)

如果一切正常的话，就大功告成了。在地图无忧利用更专业的功能特性来管理你的业务地图吧！如果遇到什么问题了，欢迎随时找小图反馈。
