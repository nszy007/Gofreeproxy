# Gofreeproxy ![](https://img.shields.io/badge/%E8%AF%AD%E8%A8%80-golang-brightgreen)![](https://img.shields.io/github/downloads/ja9er/Gofreeproxy/total) ![GitHub Repo stars](https://img.shields.io/github/stars/ja9er/Gofreeproxy)

## 
[![Stargazers over time](https://starchart.cc/ja9er/Gofreeproxy.svg)](https://starchart.cc/ja9er/Gofreeproxy)

配置好config.ini中关于fofa的参数\
usage:
>   -f	使用-f参数可读取当前目录下的proxy.txt，获取其中的代理使用\
>   -fofa  使用-fofa参数可从fofa收集资产获取公开代理使用\
>   -quake 使用-quake参数可从hunter收集资产获取公开代理使用\
>   -hunter 使用-hunter参数可从hunter收集资产获取公开代理使用\
>   -renew  当启用-fofa或-quake或-hunter参数时是否对现有proxy.txt进行重写，默认为否\
>   -CN     只请求国内的代理地址\
> -c    使用-c参数可设置验证代理的协程数量，默认为200\
> -t    使用-t参数可设置验证代理的超时时间，默认为10秒\
> -p    使用-p参数自定义本地服务端口，默认为1080\
> 成功后socks代理监听1080端口即可

效果:
![](image/img.png)

![](image/use.gif)

修改(bug)日志:
>1.增加了自定义并发数量以及代理存活验证时间 \
2.优化了控制台显示 \
3.修复了从fofa获取代理卡在98%的问题,大概是因为超时机制没生效导致卡顿 \
4.修复了mac下无法读取config.ini以及无法写入proxy.txt的问题 [[fix issues#2]](https://github.com/ja9er/Gofreeproxy/issues/2)\
5.优化控制台显示，修复了覆盖字符串未完全的bug\
![](image/proxyissus.png)
