# 终章

## 0x00

早在几个月前就应该发出来了，但下决心抛弃过去是比较难的。

我确实是娱乐圈黑客；只会水垃圾CVE的废物；祸害安全圈的废物；只会写垃圾水文的废物。

一个废物的离开也不会有什么人关心吧。

## 0x01

去年2021年7月，我刚入门Java安全，在此之前对于Java安全基本不了解，仅有一些大学应有的Java基础开发知识。对于Shiro，Fastjson，CC链等概念完全不懂，从零开始学习Java安全。

今年2022年7月，**真正学习Java安全不过一年而已**。

作为一个**普通本科**应届毕业生，我的成果如下：

### 挖到的漏洞

提交了很多漏洞，从最初鸡肋拒绝服务，到后来其他类型（一些绕过和潜在RCE）漏洞。

通过MITRE表单自行申请的垃圾CVE就不提了，只提官方发布公告的知名组件（Oracle和Apache系列等）漏洞。暂时有9个CVE，以及一些潜在漏洞。部分正在修复的RCE漏洞，可能在年底发布公告，不过那时候我已经不在了。

- Apache Log4j2 [CVE-2021-45046](https://logging.apache.org/log4j/2.x/security.html) (严重)
- Spring Framework [CVE-2022-22950](https://tanzu.vmware.com/security/cve-2022-22950) (中危)
- Oracle Weblogic [CVE-2022-21441](https://www.oracle.com/security-alerts/cpuapr2022.html) (高危)
- Apache Tomcat [CVE-2022-29885](https://lists.apache.org/thread/2b4qmhbcyqvc7dyfpjyx54c03x65vhcv) (高危)
- Apache Shiro [CVE-2022-32532](https://lists.apache.org/thread/y8260dw8vbm99oq7zv6y3mzn5ovk90xh) (高危)
- Oracle Weblogic [CVE-2022-21557](https://www.oracle.com/security-alerts/cpujul2022.html) (中危)
- Oracle Weblogic [CVE-2022-21560](https://www.oracle.com/security-alerts/cpujul2022.html) (中危)
- Oracle SOA Suite [CVE-2022-21562](https://www.oracle.com/security-alerts/cpujul2022.html) (高危)
- Oracle Weblogic [CVE-2022-21564](https://www.oracle.com/security-alerts/cpujul2022.html) (中危)
- 国内某知名开源组件的漏洞 (已确认但不允许公开)
- Spring Framework 潜在漏洞 (已修复并致谢未给CVE)
- Apache OFBIZ 潜在漏洞 (已修复并致谢未给CVE)
- 几个提交给Oralce正在修复中的漏洞 (多个产品RCE)

### 开源的项目

总计：21个项目，约**5000**左右Star

- go-sqlmap：用Golang编写的简易版sqlmap (Star最高约**150**)

- JSScan：被动分析JS内接口的burp插件 (Star最高约**50**)
- UAScan：简单的未授权访问扫描的burp插件 (Star最高约**100**)
- Gososerial：Golang生成Java反序列化Gadget库 (Star最高约**150**)
- SuperFastjsonScan：一种自动化检测Fastjson的方案 (Star最高约**50**)
- JSPHorse：利用代码混淆手段的免杀webshell生成器 (Star最高约**700**)
- ShiroMemShell：Shiro内存马注入和请求头过大的解决 (Star最高约**100**)
- CodeInspector：重写gadget-inspector以分析辅助挖洞 (Star最高约**300**
- JSPKiller：基于污点分析和模拟栈帧的webshell检测 (Star最高约**200**)
- Log4j2Scan：解析RMI和LDAP协议的无害Log4j2检测 (Star最高约**300**)
- HacLang：自己实现词法分析和语法分析的脚本语言 (Star最高约**50**)
- JNDIKit：参考JNDIExploit编写的精简版JNDI利用工具 (Star最高约**200**)
- DoSer：一种辅助挖掘拒绝服务漏洞的字节码分析工具 (Star最高约**50**)
- ShortPayload：利用字节码特性缩小反序列化Payload (Star最高约**200**)
- SpringInspector：针对Spring项目的字节码分析工具 (Star最高约**350**)
- GoBypass：集合公开众多思路的Golang免杀工具 (Star最高约**300**)
- JavaSecInterview：收集Java安全相关知识点分享 (Star最高约**1100**)
- FindShell：通过sa-jdi和JavaAgent等方式自动查杀内存马 (Star最高约**200**)
- Accelerator：通过Golang解析字节码并模拟JVM辅助挖洞 (Star最高约**50**)
- tomcat-jmxproxy-rce-exp：一种Tomcat的利用手段 (Star最高约**200**)
- CVE-2022-32532：特殊情况Shiro的权限绕过漏洞环境 (Star最高约**100**)

### 发表的安全文章

一年总计：47篇（按时间顺序：2021-7至2022-7）

- ~~CVE-2017-8046分析~~（博客，已删除）
- ~~CVE-2017-4971分析~~（博客，已删除）
- ~~CVE-2016-4977分析~~（博客，已删除）
- ~~CVE-2018-1271分析~~（博客，已删除）
- ~~CVE-2018-1270分析~~（博客，已删除）
- ~~CVE-2018-1273分析~~（博客，已删除）
- ~~CVE-2020-5405分析~~（博客，已删除）
- ~~CVE-2020-1957分析~~（博客，已删除）
- [sqlmap源码解读（1）](https://www.anquanke.com/post/id/247450)(安全客)
- [sqlmap源码解读（2）](https://www.anquanke.com/post/id/247451)(安全客)
- [sqlmap源码解读（3）](https://www.anquanke.com/post/id/247452)(安全客)
- [SpringMVC配合Fastjson的内存马利用与分析](https://www.anquanke.com/post/id/248155)（安全客）
- [CC第7链HashTable触发点深入分析](https://www.anquanke.com/post/id/248169)（安全客）
- [Golang实现RMI协议自动化检测Fastjson](https://www.anquanke.com/post/id/249402)（安全客）
- [Fastjson三种利用链对比分析](https://www.anquanke.com/post/id/248892)（安全客）
- [在MSSQL中使用CLR组件提权](https://www.anquanke.com/post/id/250346)（安全客）
- [二进制角度构造Java反序列化Payload](https://www.anquanke.com/post/id/252024)（安全客）
- [wafw00f源码浅析](https://xz.aliyun.com/t/9497)（先知）
- [几款小众web指纹识别工具源码分析](https://xz.aliyun.com/t/9498)（先知）
- [AST实现代码审计工具之入门案例](https://xz.aliyun.com/t/10287)（先知）
- [AST实现代码审计工具之SQL注入](https://xz.aliyun.com/t/10312)（先知）
- [深入分析GadgetInspector核心代码](https://xz.aliyun.com/t/10363)（先知）
- [Java自动代码审计工具实现](https://xz.aliyun.com/t/10433)（先知）
- [一处JS反调试引发的思考](https://xz.aliyun.com/t/10468)（先知）
- [浅谈加载字节码相关的Java安全问题](https://xz.aliyun.com/t/10535)（先知）
- [详解Java自动代码审计工具实现](https://tttang.com/archive/1334/)（跳跳糖）
- [探索Filter型Tomcat内存马的免杀](https://xz.aliyun.com/t/10562)（先知）
- [某知名Java框架内存马挖掘](https://forum.butian.net/share/923)（补天社区）
- [从一个被Tomcat拒绝的漏洞到特殊内存马](https://xz.aliyun.com/t/10577)（先知）
- [从Spring内存马检测到隐形马](https://xz.aliyun.com/t/10583)（先知）
- [基于污点分析的JSP Webshell检测](https://xz.aliyun.com/t/10622)（先知）
- [Apache Log4j2从RCE到RC1绕过](https://xz.aliyun.com/t/10649)（先知）
- [加载恶意字节码Webshell的检测](https://xz.aliyun.com/t/10636)（先知）
- [Apache Log4j2拒绝服务漏洞分析](https://xz.aliyun.com/t/10670)（先知）
- [浅谈Log4j2之2.15.0版本RCE](https://xz.aliyun.com/t/10689)（先知）
- [浅谈Log4j2信息泄露与不出网回显](https://xz.aliyun.com/t/10659)（先知）
- [记一次某大学渗透过程](https://xz.aliyun.com/t/10657)（先知）
- [浅谈Log4j2特殊的出网检测方式](https://xz.aliyun.com/t/10676)（先知）
- [终极Java反序列化Payload缩小技术](https://xz.aliyun.com/t/10824)（先知）
- [Agent内存马的自动分析与查杀](https://xz.aliyun.com/t/10910)（先知）
- [跟着三梦学Java安全：半自动挖洞](https://xz.aliyun.com/t/10925)（先知）
- [浅谈JSP Webshell进阶免杀](https://tttang.com/archive/1315/)（跳跳糖）
- [浅谈Spring框架CVE-2022-22950](https://xz.aliyun.com/t/11114)（先知）
- [反序列化漏洞的防御与拒绝服务](https://xz.aliyun.com/t/11288)（先知）
- ~~Tomcat CVE-2022-29885~~（博客，已删除）
- [一种Tomcat的利用方式](https://xz.aliyun.com/t/11450)（先知）
- [浅谈Shiro CVE-2022-32532](https://xz.aliyun.com/t/11501)（先知）

### B站无偿制作视频

总计：950分钟约16小时

- Pikachu靶场通关系列教学视频（共9集130分钟）
- Python安全开发系列教学视频（共12集150分钟）
- 漏洞复现与分析系列教学视频（共10集100分钟）
- 渗透工具源码分析系列教学视频（共2集20分钟）
- Burpsuite插件开发教学视频（共2集30分钟）
- 面试题解析系列教学视频（共5集70分钟）
- 二进制安全系列教学视频（共4集20分钟）
- Shiro利用与内存马教学视频（共2集30分钟）
- CC链分析教学视频（共1集10分钟）
- Fastjson自动化检测教学视频（共2集20分钟）
- Java Webshell免杀系列教学视频（共7集90分钟）
- 安全岗模拟面试辅导视频（共3集150分钟）
- 安全相关杂谈视频（共4集70分钟）
- 其他安全实战视频（共5集60分钟）

## 0x02

你多次嘲讽我写垃圾水文，确实，我承认某些文章含金量不高。但是一年不到，我写了接近50篇原创安全相关的文章。**既然你是大佬，一年内写50篇高质量原创文章不是随手就行？**

在某群多次嘲讽我只会水垃圾CVE。给你半年时间，来9个`Oracle`认可的CVE，或者9个`Apache`知名项目认可的CVE，以你这么多年的Java安全积累和经验，做到这个应该和吃饭喝水一样简单吧？**毕竟你是大佬，半年9个CVE这不是随便？**

你自称在研究创新技术，搞出来什么有意义的东西了嘛？有什么知名`RCE`是你挖出来的？哪个核弹是你挖到的？开源了什么影响行业的项目？你搞出了什么技术促进了安全的发展？**你这么强，应该有很多成果吧？**

给你一年时间，能在Github上获得**5000**多Star吗？**你是大佬，我觉得你可以轻松做到。**

你说我在B站做垃圾视频，说我割韭菜？我做B站这三四年以来，没有做过任何付费的东西，粉丝和安全圈朋友都可以证明。所以你在喷我什么？但凡我收过一分钱，你随便喷，可是我有吗？**你是大佬，无偿做几十期安全视频给新手们分享可以吗？**

## 0x03

行业内知名大佬警告我别闹大，后果我承担不起；崇拜已久的大佬让我忍着；你人脉很广，我惹不起。甚至很多师傅在那件事后拉黑了我，将我踢出了各种安全交流群。

我不敢闹大，我是垃圾废物。**如果招惹了你，在安全圈我就混不下去。**

你喷我的目的不就是要我离开？**大佬们都向着你，在逼迫我离开。**

**惹不起你，安全圈容不下我，那我退出。**

## 0x04

**我是垃圾废物吗？**

**我是。**

去年为了一份安全岗实习，拼尽了一切。

在多个平台发了十几次简历，多个群里找内推师傅。

得知面试被拒绝，花一天时间写长文只求一个机会。

我苦苦哀求面试官，只要给我机会，我可以天天加班，甚至可以不要薪资。

而面试官的回复很简单：不可能，不合适。

面试前通宵复习准备，面试后总结反思继续卷，没有一天懈怠。

好友都前往深圳，只有我一人找不到实习孤独在学校，我是垃圾废物。

托关系询问得知：HC充足，拒绝我仅因为我垃圾，太菜。

**学到身体崩溃，上吐下泻，晕倒在地，直到住院也没有得到一份实习offer。**

## 0x05

住院一个月身体好转后继续开卷，然而校招再次证明我是垃圾废物。

**在校招中，拼尽一切也拿不到一个安全岗的offer。**

想去的两个公司简历筛选被刷，确实，面试一个垃圾就是在浪费时间。

众多大厂中仅两家给了我面试机会，而我这种废物当然不可能通过了。

得知某部门没有22届校招HC后，我**不惜代价**申请延毕到23届，希望实习转正。

然而，我连一个**实习**安全研究的offer都拿不到，确实是垃圾废物。

如果是校招也就罢了，可以安慰自己：校招要求高，可这仅仅是一份**实习**；

如果HC不够也就罢了，可实际上有着**充足**的实习HC，没有其他借口；

如果经过四五次面试**最终**拒绝也就罢了，可以安慰自己运气不好，可我**一面**就凉了；

如果是二进制安全为主也就罢了，我不擅长，可这是Java安全研究。

**自以为擅长Java安全，却拿不到一份Java安全研究实习offer，我就是个笑话。**

一面都无法通过，再次证明了我是真垃圾，无论师傅们如何劝说都无法改变我是废物的事实。

我这种垃圾，不配做安全。

## 0x06

在学校，有两次，爬到最高楼层的护栏处，以为已经准备好了。

害怕中夹杂着开心，说不定跳下去我就会穿越。

可我身体在颤抖，就像菜月昴在异世界明知道可以复活也不敢跳下悬崖。

当有一天体验完所有喜欢的东西，陪伴父母老去，也就是我离开世界的时候了。

一个废物的离开，估计也没什么人关心，就当看笑话了。

## 0x07

**作为一个应届本科生，我已经拼尽全力努力了：**

- 半年内获得**9**个（以上）来自`Apache`和`Oracle`的`CVE`以及致谢。

- 超过**20**个共计**5000**多Star的安全开源项目。

- 大约**50**篇较高质量（部分水）Java安全研究文章，数十小时安全相关视频的制作。

**却连一个安全岗实习offer也拿不到，事实证明我太菜不配做安全。**

## 0x08

在退出前，我已经或者即将做的事情：

- 不会再出现**4ra1n**这个id和标志
- 我将**清空**自己的博客，但先知社区等平台的文章**保留**（收了稿费）
- 将会**清空**Github所有项目（已经关注我的师傅可以取关了）
- **删除**安全相关视频（删之前已经发动态给需要的师傅充足时间保存）
- **退出**所有安全相关的群（微信和QQ等所有社交平台）
- **删除**所有安全圈师傅好友（微信和QQ等所有社交平台）
- 关闭所有软件**添加好友**的功能
- 注销脉脉、知乎、微博等平台

另外师傅们的博客友链和爬虫等可以删除我了，删除**4ra1n**相关的一切。

我已下决心抛弃过去的一切，没有留给自己任何后路，这次是真正的离开。

至于离开后做什么，我这垃圾水平什么事也做不了，找个电动车送外卖吧。虽然苦一些，但没什么门槛，一个月也能赚三五千，凑活过日子了，能活一天是一天，等到哪天不想活了，骑车到河边跳下去一切就结束了。

