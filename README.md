# QuantumultX-
QuantumultX的配置文件，包括分流、策略组、复写、定时任务等。	

<font face="黑体">使用说明：</font> 

1、打开quantumultx,点击右下角的小风车图标  

2、滑到最下面【配置文件】-【下载】-输入配置链接  

配置链接：https://raw.githubusercontent.com/JasonNzj/QuantumultX-/main/quantumultx.conf

<font face="黑体">注意事项：</font>

1、配置文件中的【自动切换运行模式】，以我的配置文件为例：

<font color=green>#第一个filter为蜂窝网络（4g），第二个filter为其他wifi，第三项为无需科学上网的wifi名字，第四项为需全局科学的wifi名字</font>
<font color=orange>running_mode_trigger</font>=filter, filter, MI5G:all_direct, otherwifi: all_proxy
