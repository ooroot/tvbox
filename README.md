ooroot-patch-1
个人自用，请勿传播

1. tvbox配置：

（1）0707.json  OK影视多线配置接口,仅适用于Fengmi影视；

（2）0821.json  大而全的配置，在饭太硬配置的基础上添加了若干优质点播源、直播线路和解析；

（3）0822.json  极简配置，OK大佬的jar，还包括几条路飞、俊于的源。

（4）0825.json  小而精的配置，jar包来源于Panda Groove的go包，其中泥巴、星星等，需要替换成自己的代理url；

（5）0826.json  完全来源于饭太硬的jar包和配置；

（6）0827.json  jar包和配置来源于fongmi；

（7）0828.json  jar包和配置来源于唐三；

（8）js.json  jar包来源于Panda Groove的go包，资源来源于道长drpy(js)仓库 添加 YouTube 直播；

（9）XBPQ.json  XBPQ源，jar包和配置来源于小米小爆脾气；

（10）XYQ.json  XYQ源，jar包和配置来源于香雅情；

（11）cat.json  cat源，资源来源于网络各路大佬。/cat/js配合猫影视可直接食用；

（12） jsm.json 来自js.json + 0826.json 合集 家庭电视可用 删除YouTube 直播，OK影视 可用 电视建议使用OK影视 https://github.com/FongMi/Release 支持多直播选择。
 暗号:9918 991880

（1）OK影视版本  项目地址：<https://github.com/FongMi/TV> 支持直播多线路、自动换源、直播倍速，手机投屏；

（2）q215613905版本  项目地址：<https://github.com/q215613905/TVBoxOS> 支持直播回放；

（3）takagen99版本  项目地址：<https://github.com/takagen99/Box> 支持直播回放，界面美观；

（4）皮皮虾版本  发布频道：<https://t.me/pipixiawerun> 支持直播回放，支持弹幕；

（5）新版猫影视   项目地址：<https://github.com/catvod/CatVodOpen> 界面简洁，支持多平台。

（6）手机版本  项目地址：<https://github.com/XiaoRanLiu3119/TVBoxOS-Mobile> 竖屏


```json
{
"token":"这里填写阿里云盘的32位token,也可以不填写,在播放阿里云盘属性时会弹出窗口,点击QrCode,用阿里云盘app扫码",
"open_token":"这里填写通过alist或其他openapi提供方申请的280位aliyun openapi token,也可以不写,会自动隐藏转存原画",
"thread_limit":32,//这里是阿里云盘的GO代理的并发协程数或java代理的并发线程数,若遇到账号被限制并发数,请将此数值改为10
"is_vip":true,//是否是阿里云盘的VIP用户,设置为true后,使用vip_thread_limit设置的数值来并发加速。如本设置项目不是true,则自动隐藏"转存原画"
"vip_thread_limit":10,//这里是阿里云盘的转存原画（OpenToken）并发线程数,若遇到账号被限制并发数,请将此数值改为10
"quark_thread_limit":32,//这里是夸克网盘GO代理的并发协程数或java代理的并发线程数,若遇到账号被限制并发数,请将此数值改为10
"quark_vip_thread_limit":16,//这里是夸克网盘设置quark_is_vip:true之后的并发线程数,若遇到账号被限制并发数,请将此数值改为10
"quark_is_vip":false,//是否是夸克网盘的VIP用户,设置为true后,线程数受quark_vip_thread_limit控制
"vod_flags":"4k|4kz|auto",//这里是播放阿里云的画质选项,4k代表不转存原画（GO原画）,4kz代表转存原画,其他都代表预览画质,可选的预览画质包括qhd,fhd,hd,sd,ld,
"quark_flags":"4kz|auto",//这里是播放夸克网盘的画质选项,4kz代表转存原画（GO原画）,其他都代表转码画质,可选的预览画质包括4k,2k,super,high,low,normal
"uc_thread_limit":0,
"uc_is_vip":false,
"uc_flags":"4kz|auto",
"uc_vip_thread_limit":0,
"thunder_thread_limit":0,
"thunder_is_vip":false,
"thunder_vip_thread_limit":0,
"thunder_flags":"4k|4kz|auto",
"aliproxy":"这里填写外部的加速代理,用于在盒子性能不够的情况下,使用外部的加速代理来加速播放,可以不填写",
"proxy":"这里填写用于科学上网的地址,连接openapi或某些资源站可能会需要用到,可以不填写",
"open_api_url":"https://api.xhofe.top/alist/ali_open/token",//这是alist的openapi接口地址,也可使用其他openapi提供商的地址。
"danmu":true,//是否全局开启阿里云盘所有csp的弹幕支持,聚合类CSP仍需单独设置,例如Wogg,Wobg
"quark_danmu":true,//是否全局开启夸克网盘的所有csp的弹幕支持,聚合类CSP仍需单独设置,例如Wogg,Wobg
"quark_cookie":"这里填写通过https://pan.quark.cn网站获取到的cookie,会很长,全数填入即可。",
"uc_cookie":"这里填写通过https://drive.uc.cn网站登录获取的cookie",
"thunder_username":"这里填入用户名或手机号,如果是手机号,记得是类似'+86 139123457'这样的格式,+86后有空格才对",
"thunder_password":"密码",
"thunder_captchatoken":"首次使用迅雷网盘时,需要使用app弹出的登陆地址去接码登录,并获取captchaToken,具体方法参考alist网站的文档:https://alist.nn.ci/zh/guide/drivers/thunder.html",
"pikpak_username":"PikPak网盘的用户名",
"pikpak_password":"PikPak网盘的密码",
"pikpak_flags":"4k|auto",
"pikpak_thread_limit":2,
"pikpak_vip_thread_limit":2,
"pikpak_proxy":"用于科学上网连接PikPak网盘的代理服务器地址"
}
```
