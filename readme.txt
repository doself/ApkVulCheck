﻿安卓漏洞扫描工具简介
0x1目前支持的漏洞类型：
1、任意文件读写漏洞
2、密钥硬编码漏洞
3、强制类型转换本地拒绝服务漏洞
4、系统组件本地拒绝服务漏洞
5、Intent Schema URL漏洞
6、Content Provider组件本地SQL注入漏洞
7、代码动态加载安全检测
8、证书弱校验
9、主机名弱校验
10、HTTPS敏感数据劫持漏洞
11、Hash算法不安全
12、AES弱加密
13、Locat泄露隐私信息
14、日志泄漏风险
15、PendingIntent误用风险
16、Intent隐式调用
17、数据库文件任意读写
18、WebView系统隐藏接口漏洞检测
19、WebView组件远程代码执行漏洞检测
20、WebView忽略SSL证书错误检测
21、WebView明文存储密码
22、SharedPreferences任意读写
23、任意文件读写
24、随机数使用不安全
25、组件权限检查
26、应用是否可调式检查
27、应用权限检查
28、应用自定义权限检查
30、应用备份漏洞检查

0x2 使用方法：
1、将需要扫描的apk文件放到workspace/apk目录下
2、点击AndroidCodeCheck.exe或执行python AndroidCodeCheck.py即可执行漏洞扫描

0x3 报告输出
报告输出路径在report下
1、txt格式
算是程序的运行日志吧，也可以作为扫描结果参考。
2、html格式
html格式的报告有目录，点击目录中的漏洞名称即可跳转到相应的漏洞类型说明。在类型说明处可点击返回目录返回到漏洞
目录列表，方便漏洞审阅。

0x4 更新说明
1、.5版本主要优化了apk处理，之前需要手动提取dex文件，现在可以自动提取分析了。用户只要
将apk文件放到workspace的apk文件夹目录下，然后运行引擎程序即可执行静态扫描操作。
2、新版本支持多个apk进行静态扫描分析，只要将需要扫描的文件全部放到apk文件夹下即可
3、优化了下项目目录，使之更加的规范化。

2018/8/1更新说明
增加了对manifest.xml文件的解析，据此获得apk文件的一些信息，包括：
1、包名信息
2、申请的权限信息
3、自定义的权限信息
4、组件信息，包括四大组件（activity，service，receiver，provider）
漏洞判断主要增加了：
1、针对activity，service，receiver，provider四大组件的导出属性进行判断
2、增加了备份漏洞的判断

更新备忘录
2018/8/2更新说明
增加了对应用是否可调式的判断
2018/8/2更新说明
增加了对应用加固类型识别的插件
现在支持的识别厂商有：
娜迦
娜迦企业版
爱加密
爱加密企业版
梆梆免费版
360
通付盾
网秦
百度
阿里聚安全
腾讯
腾讯御安全
网易易盾
APKProtect
几维安全
顶像科技
盛大
瑞星

2018/8/27
1、添加了一个针对webview隐藏api检测模块
2、优化扫描检测逻辑
3、优化项目结构
如果你有什么建议愿意交流一下，请联系我：
qq:747289639
email:747289639@qq.com
