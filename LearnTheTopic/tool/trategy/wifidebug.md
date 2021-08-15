在开发的过程中只提供了一个USB接口，但是USB需要被其他设备占用，这个时候如果要调试，就需要使用无线adb调试。

通过串口设置链接。串口模式下：

串口输入 setprop service.adb.tcp.port 5555 && stop adbd && start adbd && netcfg

然后adb connect 　ｉｐ
setprop service.adb.tcp.port 5555   //设置监听的端口，端口可以自定义，如5554，5555是默认的

stop adbd   //关闭adbd

start adbd   //重新启动adbd

ＵＳＢ连接的模式下　：

1、 确保电脑和Android设备连接在同一个WIFI网络环境。

2、 用USB线连接Android设备。连接上之后你的电脑就会检查到设备并且ADB将会以USB模式启动。可以通过adb devices命令检查连接上的设备，用adb usb命令确认adb是运行在usb模式下面。
