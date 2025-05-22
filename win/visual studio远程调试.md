# Visual Studio Debug ：远程调试
1、安装 Remote Debugger
方法一：
从微软官网下载远程工具。

注意，一定要安装与 VS 版本和目标机操作系统匹配的远程工具。

例如，你用的是 VS2017，就要下载 VS2017 版的远程工具，另外，还要考虑目标机操作系统位数，是 32 位就要安装 32 位远程工具，是 64 位就要安装 64 位远程工具。

下载地址从这里找吧：

Remote debugging in Visual Studio： https://link.zhihu.com/?target=https%3A//docs.microsoft.com/zh-cn/visualstudio/debugger/remote-debugging

方法二：

这是一个更为简单的方法。

在你本地的 VS 安装目录下找到 msvsmon.exe，此文件就是 Remote Debugger。
这里同样需要注意，要与目标机的操作系统位数匹配。
2. 配置 Remote Debugger
这一步还是在目标机上。

所在登陆账户，一定要拥有管理员权限。

打开安装好的 Remote Debugger (msvsmon.exe)，首次打开时，会出现配置窗口，提醒配置一些参数。

只需要配置一次，再次打开时，不会弹出该窗口。
![image](https://github.com/user-attachments/assets/de77b088-07d8-46b9-a5ce-01f79fba6b12)

# 附件
## 参考资料
https://blog.csdn.net/thebulesky/article/details/120852560
