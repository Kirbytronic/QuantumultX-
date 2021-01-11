# QuantumultX-
QuantumultX的配置文件，包括分流、策略组、复写、定时任务等。	

使用说明：

1、打开quantumultx,点击右下角的小风车图标  

2、滑到最下面【配置文件】-【下载】-输入配置链接  

配置链接：https://raw.githubusercontent.com/JasonNzj/QuantumultX-/main/quantumultx.conf

3、回到首页，再次点击小风车，在【节点】-【引用（订阅）】，点击右上角+，写入你的机场订阅，如显示失败请勾选上资源解析器，若仍有错误请检查自己的链接是否为QX所识别的格式。

4、回到首页在【自定义策略】中配置自己的节点。若下面的HK Server、US Server等没有节点信息，请到最上面PROXY下面检查自己的节点信息里面是否包含HK、US等关键字

 地区策略组中的关键字匹配在【配置文件】-【服务器按地区分组策略(正则策略)】中，请按照格式进行修改，支持正则表达式。


注意事项：

1、配置文件中的【自动切换运行模式】，以我的配置文件为例：
````diff
+  #第一个filter为蜂窝网络（4g），第二个filter为其他wifi，第三项为无需科学上网的wifi名字(如果你有软路由并配置了科学上网，请把MI5G改成你自己wifi的名字)，第四项为需全局科学的wifi名字
-  running_mode_trigger=filter, filter, MI5G:all_direct, otherwifi: all_proxy
2、配置文件中的【server_remote】是你的订阅信息，订阅机场的链接后，你的服务器配置会在这里
3、关于定时任务的注意事项：
1、点击右下角小风车，找到【构造请求】
2、请求列表中的 汇率监控、疫情日报是无需配置的，其中b站签到需要先在浏览器中登陆账号获取cookie，贴吧、美团、联通需要到各自的app中进行签到操作以获取cookie，其他的脚本请务必点开查看脚本中的注意事项，配合boxjs使用。
