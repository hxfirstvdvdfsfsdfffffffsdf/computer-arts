
     计算机本身有很多好用的实用技巧，通过这些技巧可以方便我们的计算机使用，不管是计算机相关行业还是非相关行业都应该熟悉，毕竟现在笔记本几乎成为了上班的标配。

     接下来我会将自己这些年总结出的一些实用技巧分享给大家.

I. 电脑自带快捷截图（支持任意格式截图、全屏截图和延时截图,还可以支持图片编辑，唯一不足是不支持滚动截屏）：
    在我大学的时候时常为截图感到烦恼，因为做网上作业的时候经常会上传很多的截图，但是下载的截图工具其实并不方便，而且还要安装，每次还要打开和关闭，感觉都不太满意 E^E

于是我决定找一个最简单的方法做出让自己满意的截图操作，经过在网上大量搜索后发现win确实自带了很多实用的功能，只是这些功能不被众人知晓而已，其中就包括电脑自带的快速截图工具：snippingtool

具体步骤：

                 win+r 进入运行界面
                 运行界面输入 snippingtool  命令
                 在界面上进行截图操作


II.查看电脑曾经成功连接过的wifi密码
你是否还在为突然忘记成功连接过的wifi密码而无法上网担忧？看到这里就不用担心了，废话不说了，直接安利了！

   win +r
   输入cmd
   命令行中输入如下命令：

 netsh wlan show profiles   会显示所有曾今成功连接过的wifi名称

 接着输入命令netsh wlan show profile name=?  key=clear,  其中的name就是上面的wifi名称，key=clear表示明文显示密码：

 输入后密码就会包含在信息中一起输出
 
III  重置网络底层设置

在我大二的时候，有一个大一的学妹的电脑出了问题，她希望我可以给她修一修，不然她就要去计算机维修中心去维修，会多花一笔钱，于是我接过她的戴尔电脑，发现当计算机连接无线网络时虽然网络是不加密或者密码知道但是屏幕右下角还是有红×提示连接出错，最后我在网上找了很久，才发现电脑很可能是winsock层的网络连接出了问题，最后在命令行通过输入netsh winsock reset命令对winsock层进行了重置，重启之后一切都正常了，这件事我印象蛮深的，我也一直记着这个命令。但是用这个命令一定要谨慎，netsh winsock reset确实可以解决多数网络连接问题，但是却是以重置winsock层的相关配置为代价的。


 
