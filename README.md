# dyhNote
在 Spring Boot 应用程序中，当你使用 -Dspring.profiles.active=sit 参数启动应用时，Spring 会优先加载对应环境的配置文件（在这种情况下是 application-sit.yml）。不过，application.yml 文件仍然会被加载，因为它被视为默认的基础配置文件。

具体来说，Spring Boot 的配置加载过程大致如下：

基础配置文件：总是会加载 application.properties 或 application.yml 文件的内容，即使指定了环境配置文件也是如此。这是为了提供一个通用的基本配置集。
环境特定配置文件：如果指定了环境（如通过 -Dspring.profiles.active=sit），则会加载与该环境相关的配置文件（即 application-sit.yml）。这些配置文件中的属性会覆盖基础配置文件中的同名属性。
因此，在你的例子中，application.yml 和 application-sit.yml 都会被加载。application-sit.yml 中的配置会覆盖 application.yml 中相同名称的配置项。这样做的好处是可以保持基本配置的一致性，同时允许每个环境有不同的定制化配置。

一、信息收集
IP定位/真实IP：
https://www.ipuu.net/#/home
https://www.opengps.cn/Data/IP/ipplus.aspx

https://site.ip138.com/

 https://securitytrails.com/

多个地点PING：
多个地点ping服务器-网站测速-站长工具 (chinaz.com)

 Website uptime monitoring service, check is site down - Host-tracker

网页测试 - 网站性能和优化测试 (webpagetest.org)

 Website Speed Test | Pingdom Tools

                                网站测速|网站速度测试|网速测试|电信|联通|网通|全国|监控|CDN|PING|DNS 一起测试|17CE.COM

 Whois信息查询：

域名Whois查询 - 站长之家

 https://whois.aliyun.com/

 https://who.is/

TLS证书查询：

https://censys.io

 亚数信息-SSL/TLS安全评估报告

IP反差域名：

微步在线X情报社区-威胁情报查询_威胁分析平台_开放社区

  https://www.virustotal.com/  

http://www.myipneighbors.com/

 http://www.rootkit.net.cn/index.aspx

 IP/IPv6查询，服务器地址查询 - 站长工具

 https://dns.aizhan.com/
Network Tools by YouGetSignal.com

DNS查询：

https://dnsdb.io/zh-cn

 微步在线X情报社区-威胁情报查询_威胁分析平台_开放社区

Ping.cn-DNS在线查询工具

指纹识别：
yunsee.cn-2.0
御剑web指纹识别 – WebShell'S Blog

在线指纹识别,在线cms识别小插件--在线工具 (bugscaner.com)

WAF识别：GitHub - stamparm/identYwaf: Blind WAF identification tool

目录扫描：GitHub - maurosoria/dirsearch: Web path scanner

子域名爆破：GitHub - knownsec/ksubdomain: 无状态子域名爆破工具

弱口令/密码：https://github.com/shack2/SNETCracker

 HTTP参数：https://github.com/s0md3v/Arjun

信息泄露：

git泄露利用脚本：https://github.com/lijiejie/GitHack     

GitHub 泄露监控系统：https://github.com/0xbug/Hawkeye

电子邮箱：邮箱地址搜索 Find email addresses of companies and people - Skymem

网络测绘：https://securitytrails.com/      Censys Search 

网络空间：

https://fofa.info/ 零零信安 | ASM | 攻击面 | 外部攻击面管理专家 | 比攻击者更快一步了解您自己的风险

登录 - 360网络空间资产测绘

Shodan Account        

鹰图平台 

Soall Search Engine

知风-互联网联网工控资产与企业分析系统   

资产查询：

爱企查首页 - 专业企业查询平台 - 查企业 - 查老板 - 查风险 - 工商信息查询系统   

 企查查 - 企业工商信息查询系统_查企业_查老板_查风险就上企查查!  

小蓝本-商业信息搜索

信息泄露：

全国移动电话卡“一证通查”  

 https://loseprivacy.xyz/login.html



二、漏洞整理
漏洞利用数据库：

https://www.exploit-db.com/

 Vulnerability & Exploit Database

知道创宇漏洞平台：https://www.seebug.org/

乌云历史漏洞查询：乌云(WooYun.org)历史漏洞查询---http://WY.ZONE.CI

工控漏洞库：

http://vulhub.org.cn/view/ics

  工控漏洞子库

工控安全：灯塔实验室 – 专注于工控安全攻防技术研究-ICS Security Workspace

工控安全信息下载中心：工控安全 搜索结果 附件下载,信息安全知识库 vipread.com

三、渗透工具
沙箱：

hs大圣云沙箱检测系统

VirusTotal

工具：

在线工具 - Bugku CTF

在线文本去重复工具 - 在线工具

headers转字典(dict)-在线工具

在线域名网址整理 - 在线工具

免费短信验证码接收平台导航--在线工具

Sign in - start.me

Windows杀软在线对比辅助-MaiKeFee

IP定位、WiFi精确查询：

https://met.red/



四、加密解密
MD5:

md5在线解密破解,md5解密加密

MD5免费在线解密破解_MD5在线加密-SOMD5

编码：CTF在线工具-CTF工具|CTF编码|CTF密码学|CTF加解密|程序员工具|在线编解码

彩虹：https://www.objectif-securite.ch/ophcrack

五、网络靶场
WgpSec CTF

Vulnerable By Design ~ VulnHub

Hack The Box: Hacking Training For The Best | Individuals & Companies

BUUCTF在线评测

六、安全文库
Hacking8 安全文库 - 像黑客一样学习

https://nosec.org/home/index

全部 - 文章 - 奇安信攻防社区

T00ls | 低调求发展 - 潜心习安全 - T00ls.Com

安全客 - 安全资讯平台

先知社区

Paper
————————————————

                            版权声明：本文为博主原创文章，遵循 CC 4.0 BY-SA 版权协议，转载请附上原文出处链接和本声明。
                        
原文链接：https://blog.csdn.net/weixin_68057794/article/details/126903890
