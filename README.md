·此dump1090-baidu项目是由antirez@gmail.com的项目改编。
·专门为无法访问谷歌地图的用户改编，地图API接口由谷歌地图接口换成百度地图。
·如果认为侵权，请留言。
·感谢原作者<antirez@gmail.com>


前提：
需要安装librtlsdr-dev ， rtl-sdr
apt-get install librtlsdr-dev
apt-get install rtl-sdr

安装
输入“make”。

正常使用
要直接从RTL设备捕获流量并在标准输出上显示捕获的流量，只需运行没有选项的程序：

./dump1090
要输出十六进制消息：

./dump1090 --raw
要以交互方式运行程序：

./dump1090 --interactive
要以交互模式运行程序，并提供网络支持，并使用浏览器连接到http：// localhost：8080以查看实时流量：

./dump1090 --interactive --net
在交互模式下，可以拥有较少的信息密集但更多的“街机风格”输出，其中屏幕每秒刷新一次，显示所有最近看过的飞机，其中包含从接收到的模式S中提取的一些附加信息，如高度和航班号。
