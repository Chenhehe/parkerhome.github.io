### mac安装vscode出现错误There was an error in starting the debug server. Error = {"code":"ENOTFOUND","errno":"ENOTFOUND","syscall":"getaddrinfo","address":"localhost"}

在使用mac系统运行vscode搭建python环境，并且进行代码的调试时出现错误：
There was an error in starting the debug server. Error = {"code":"ENOTFOUND","errno":"ENOTFOUND","syscall":"getaddrinfo","address":"localhost"}

问题原因：
本地未进行 127.0.0.1	localhost  的host解析，而python调试时需要，导致报错。

解决办法：
在本机进行 127.0.0.1	localhost 解析。

解决办法原文链接：
[点击这里看原文链接](https://github.com/Microsoft/vscode-python/issues/715)