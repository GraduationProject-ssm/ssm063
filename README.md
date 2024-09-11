# [首页查询更多项目](https://github.com/GraduationProject-ssm) 包安装运行


# ssm063基于SSM框架的德云社票务系统的设计与实现+vue

![picture](https://raw.githubusercontent.com/GraduationProject-springboot/.github/main/img/wx.png)

### 点击播放视频 ▼
[![Watch the video](https://i.sstatic.net/Vp2cE.png)](https://www.bilibili.com/video/BV1T48XecE9G?p=61)


# 第1章 绪论
## 1.1 课题背景
在中国经济的快速发展下，各行各业都随之发展，快速进步，从而提升了人们的生活质量，带来了消费市场的活跃。除了必要的生活需求外，人们开始重视生活品质，包含了身体健康和精神文化的需求。现代生活水平的提高，人们的生活不仅仅只追求物质生活，更高的倾向于精神的享受。近年来，德云社的蓬勃发展，相声受到了人们的喜欢，人们对德云社订票的需求在不断的增大，让传统的德云社订票模式已经无法满足用户的需求，费事费力。在这样的情况下，我们开发了德云社票务系统，为人们提供大量的票务信息，让用户很好的掌握相声票务信息，尤其解决了排队购票的现状，让人们享受不需排队购票的服务，通过网络简单快捷订票，足不出户就可以网上订票，查询相声票务信息，进行购买操作。本系统的开发更有利于德云社更快更好的发展。

本课题德云社票务系统有着无法比拟的优点，其具有利用率高的特点，同时使得用户更快的订票，受到了人们的广泛使用；同时德云社票务系统利用计算机平台，对信息进行管理，储存空间大，成本低，查找方便等。德云社票务系统，采用MYSQL数据库，充分保证数据的安全性、稳定性，管理员可以快捷准确的管理票务相关信息。
## 1.2  设计原则
在开始开发项目之前，必须要先考虑项目的实用性、科学性，以及该项目是否能够真正让用户受益并尽可能的发挥项目的作用。因此，在开发前，通过以下几条原则对项目进行判断：

（1）可行性原则。项目需要保证经济可行性和技术可行性，这包括了项目在浏览端、服务端等方面上的经济和技术上是可以达成的。

（2）适应性原则。项目要保证可维护性和可扩展性，这是每个非短期项目都需要考虑的，并且不论是维护还是扩展，都必须要建立在适应用户的正常需求的基础上。

（3）安全性及保密性原则。要充分保证用户信息的安全性和保密性，不能因为开发上的疏忽，导致用户的信息泄露。

（4）系统工程原则。为了确保项目的整体性，在项目调查、项目分析、项目设计、项目开发的过程中，都需遵从项目工程的方法和步骤逐步进行。

（5）统一规划、分期实施、逐步完善原则。项目开发的过程中，要按照规划、分期实施，特别是要注意在项目开发过程中要有条理，从点到面，一步步完善，不要贪图进度，要循环渐进的对项目进行开发。
## 1.3  论文组织结构
第一章主要是简单的介绍下设计本网站的研究背景和设计原则，在这一章里主要是让大家了解下我的设计的前因后果，为接下来我的其它章节做铺垫。

第二章主要是介绍在设计过程中所涉及到的技术。

第三章主要是介绍下设计这个网站所需要的需求以及我们的功能需求分析，因为只有更好的分析清楚我们的功能需求才能更好的完成我们的设计。

第四章网站系统设计，主要介绍了网站结构的设计以及展示了数据库E-R图设计，这一章主要是为了能让大家更好的了解网站的一些基本设计信息。

第五章系统的实现，介绍了系统每个模块的设计与实现，让大家能清晰的了解系统的主要功能。

第六章系统的测试，这章主要是测试下各个部分每个功能是否能用，看下是否有错误。

第七章系统总结，进行系统最后的总结工作。
#
1
# 第2章  关键技术简介
## 2.1 Java技术
Java是一种非常常用的编程语言，在全球编程语言排行版上总是前三。在方兴未艾的计算机技术发展历程中，Java的身影无处不在，并且拥有旺盛的生命力。Java的跨平台能力十分强大，只需一次编译，任何地方都可以运行。除此之外，它还拥有简单的语法和实用的类库，让编程人员可以尽可能将精力集中在问题的求解上，并且许多开源项目和科研成果都是采用它实现的。

在1995年这一年的5月份，著名的Sun Microsystems公司在程序开发设计上面郑重推出一种面向对象开发的程序设计语言——Java，最开始的时候Java是由詹姆斯.高斯林这位伟大的JAVA之父来进行主导，但是在后来由于各种原因，让甲骨文公司这个针对商业程序创建了oracle大型数据库的公司收购了Java。Java的平台总共算下来有3个，分别为javaME和javaSE以及javaEE这3个java平台。下面将对其进行分别介绍。

（1）在电脑桌面程序的开发上面需要选择JavaME，这个用得也比较多。

（2）企业也会根据工作以及业务需要开发各种软件，那么就会选用JavcEE这个支持企业版软件的开发的Java平台，JavcEE主攻运用在企业领域上面的web应用，JavcEE也在javaSE的基础上获得了比如jsp技术 ，Servlet技术等程序开发技术的支持。

（3）现在生活中手机的普及化，也使得手机端这样的移动设备的软件的兴起，JavaME这个迷你版java平台就能运用于移动端的软件开发操作。
## 2.2 B/S结构
此次设计的网络结构模式B/S结构（Browser/Server）。B/S架构也称为B/S模式，是一种服务器以及浏览器架构模式。B/S的工作模式都是先由浏览器请求，服务器再响应。B/S体系结构解决了异构系统中的连接难题，大大改善了系统的开放性，让系统的扩展和维护更加简单；同时，B/S体系结构操作也比较容易，界面全都为浏览器模式，容易分发数据的捕获程序。只要安装通用的浏览器（如WWW浏览器）就能通过Web服务器与数据库进行数据交互。此结构的好处之一在于由于它使用的统一的浏览器，使其可以在不同的地方且不需要用专门的软件进行操作，实现了不论你使用怎样的接入网的方式都可以对公共的数据进行调用和浏览。

相对于C/S模式，B/S模式是对C/S模式应用的扩展，B/S模式不用对不同的计算机安装不同应用程序，还有安全性的要求及对模式上手难度都比前者更好。B/S模式可以让客户机的压力大大减轻，工作的负荷被合理的分配了。

B/S三层框架结构图如图2-1所示：

显示逻辑

浏览器

事物处理逻辑

Web服务

数据库

事物处理逻辑

数据库服务器

响应

请求

相应

请求

求

![](/md/blog.001.png)

图2-1 B/S三层框架结构图
## 2.3 MYSQL数据库
MySQL 是关系型数据库管理系统的代表， 因为MySQL是其免费开源的，而且MySQL的功能已经足够用对于学习和中小型企业来讲，所以开发中小型网站都会选择MySQL作为网站的数据库。[13]

MySQL具有开放性，它是一种关系型数据库管理系统，并且它的源代码可以被大众所熟知[3]。由于MySQL是开放源代码的，因此，只要经过授权就可以在自己需求的基础上对其进行修改。MySQL因为其固有的特点而备受关注，它具有很强的适应性，并且十分可靠，查询速度快。MySQL安装起来非常方便，且数据存储量大，不需要事务化处理。Sql语言拥有很多的方法，在项目中编写sql语句时使用起来是非常方便的，不会像其他语言那样需要编写更多的语句。正因为MySQL使用sql语言进行数据库管理，所以它收到了大多数程序员的热爱。
## 2.4 SSM框架
本德云社票务系统基于Spring、SpringMVC、Mybatis框架进行开发设计。

Spring 框架是在2004年首次发布，之后出现了多次的重大修订。Spring框架是由七个不同的模块组成，分别是SpringCore、Spring AOP、Spring ORM、Spring DAO、Spring Web Flow、Spring Context和Spring Web MVC[2]。这些模块提供不同的平台来开发不同的企业应用程序 ，本课题使用Spring Web MVC模块开发基于MVC的应用程序。

Spring Web MVC是基于Servlet API的原始Web框架，从一开始就包含在Spring 框架中。“Spring Web MVC”是该框架的正式名称，但通常被简称为“Spring MVC” [3]。Spring MVC框架提供了模型模块-视图模块-控制器的架构和可用于直接开发的Web应用程序的现成组件。Spring MVC模式将应用程序的不同方面分开，使元素之间形成松散耦合。

MyBatis原名叫做iBatis属于持久层框架，消除了大部分JDBC代码和参数的设置以及结果集的检索。这个框架不仅支持普通SQL查询和存储过程，还支持高级的映射[4]。MyBatis使用.xml和注解来做原始映射和配置，将接口和Java对象映射成数据库记录。

#
# 第3章 系统分析
## 3.1 可行性分析
在系统开发之初要进行系统可行分析，这样做的目的就是使用最小成本解决最大问题，一旦程序开发满足用户需要，带来的好处也是很多的。下面我们将从技术上、操作上、经济上等方面来考虑这个系统到底值不值得开发。
### 3.1.1 技术可行性
本德云社票务系统采用Java和MYSQL数据库进行开发设计，作为计算机专业学生，在学校期间就接触到许多关于编程方面的知识，当然也包括各种编程软件，对他们的了解度也比较系统，所以技术开发上面还是有一定把握。
### 3.1.2 经济可行性
由于自己本身就是学生，还没有正式参加工作，金钱上面一直都处于缺乏状态。所以在开发程序过程中，我是不会花太多经济成本在上面的。针对开发软件和数据库，还有界面设计的photoshop软件等在百度上面就可以直接下载，然后根据各种安装视频进行安装，这些资源都是免费的，程序编码阶段使用的源代码在百度上面可以轻松获得，在有网络的环境下就能下载下来，不需要支付任何费用，经济成本很低。
### 3.1.3 操作可行性
本人自己就是学生，程序开发经验不足，在界面设计上面不会设计太复杂，要讲究简单好看，操作上要方便，不能让用户觉得不流畅。用户一旦进入操作界面，界面上就会有相应提示，跟着操作提示就可以找到对应的功能操作模块，对于用户来说免培训就能使用。本德云社票务系统本身具有操作可行性，其界面设计清晰、功能权限分配合理，操作简单，不同用户登录后可对进行相应功能模块的操作，具有极高的操作可行性。
### 3.1.4 时间可行性
从时间上看，在三个月的时间里学习相关知识，开发本德云社票务系统，时间上是有点紧，但是不是不可能实现，在做毕业设计的这几个月里，我通过努力使得功能应该基本可以实现。

综上所述，我们进行了四个方面的可行性研究，可以看出，该基于SSM框架的德云社票务系统的开发是没有问题的。
## 3.2 系统功能分析
本基于SSM框架的德云社票务系统主要满足两种用户的需求，这两种用户分别为管理员和用户，用户间的静态结构图如图3-1所示。

![](/md/blog.002.png)

图3-1 用户间静态结构图

（1）管理员：管理员登录后可对系统进行全面的管理，主要功能模块包括个人中心、会员管理、票务信息管理、常见问题管理、管理员管理、系统管理（轮播图管理、公告信息、问题反馈）以及订单管理。管理员用例图如图3-2所示。

![](/md/blog.003.png)

图3-2 管理员用例图图

（2）用户：用户进入本系统可查看票务信息、常见问题、公告信息等，注册登陆后主要功能模块包括票务预订、问题反馈、个人中心、我的订单、我的地址、我的收藏等。用户用例图如图3-3所示。

![](/md/blog.004.png)

图3-3 用户用例图
## 3.3 系统性能分析
（1）系统的存储性：因为是德云社票务系统，所以就会在数据库要求上比较严格，信息录入的比较多，而且丰富复杂， 这就需要一个强大的数据库来存放更多的数据和保证数据的时时性。

（2）系统的易学性：系统设计的应该简单易学的，设计的各种功能应该简单操作，不需要努力学习培训，缩短用户熟悉系统的进程。

（3）系统的数据要求：数据应该录入准确，需要更新时，数据应该可以及时的修改，数据还应该有独立保存，不能删除数据的时候会连带着把还需要的数据都删除掉。

（4）系统稳定性：开发的德云社票务系统要求运行稳定，运行过程中无界面不清楚、字体模糊等现象。

（5）系统可靠性：系统不可以有病毒类代码，必须有拦截器，验证方法，对里面信息的保护措施，这样才让人用的放心。
## 3.4 系统流程分析
### 3.4.1注册流程
未有账号的用户可进行注册操作，在注册时系统会判断用户名是否已存在，已存在的话，提示返回重新填写用户名，用户名不存在，填写其他注册信息，系统判断注册信息是否正确，正确则在数据库中添加用户信息，注册成功。用户注册流程图如图3-4所示。

![](/md/blog.005.png)

图3-4注册流程图
### 3.4.2登录流程
为了保证系统的安全性，要对本德云社票务系统进行管理，必须进行管理员登录，否则无权进行系统管理，同时用户要想实现在线选座订票等操作，也必须登录系统。用户登录流程图如图3-5所示

![](/md/blog.006.png)

图3-5登录流程图
#
# 第4章  系统设计
## 4.1 系统结构设计
系统结构设计是一个将一个庞大的任务细分为多个小的任务的过程，这些小的任务分段完成后，组合在一起形成一个完整的任务。在整个设计过程，以确定可能的具体方案达成每一个小的最终目标，对于每一个小的目标而言，我们必须先了解一些相关的需求分析的信息。然后对系统进行初步的设计，并对其逐渐进行优化，设计出一个具体可实现的系统结构。

本基于SSM框架的德云社票务系统主要包括用户模块和管理员模块，根据第三章中系统功能需求分析，可画出本德云社票务系统的结构图如图4-1所示：

![](/md/blog.007.png)

图 4-1  系统结构图
## 4.2系统顺序图
### 4.2.1登录模块顺序图
用户和管理员均可进行登录操作，登录模块的顺序图如图 4-2 所示。

![](/md/blog.008.png)

图4-2用户登录顺序图
### 4.2.2添加信息模块顺序图
管理员和用户登录后均可进行添加信息操作，添加信息顺序图如图4-3所示

![](/md/blog.009.png)

图4-3添加信息顺序图
## 4.3 数据库设计
一个好的数据库可以关系到程序开发的优劣，数据库设计离不开表结构的设计，还有表与表之间的联系，以及系统开发需要设计的数据表内容等信息。在进行数据库设计期间，还是需要多花时间进行考虑，最终设计出配套程序的数据库出来。
### 4.3.1 数据库E-R图设计
本德云社票务系统采用的是MYSQL数据库，数据存储快，因为德云社票务系统，主要的就是对信息的管理，信息内容比较多，这就需要好好的设计一个好的数据库，分类要清楚，不能添加信息的时候，造成信息太过混乱，设计好的数据库首先就需要先把各个实体之间的关系表达明确，下面我们用E-R图来具体表示。

E-R图是一种描述显示数据类型间的关系的数据描述方法，E-R图可以完整地映射出现实模型的关系。E-R图中的三个最为重要的元素就是实体、属性、关系。E-R图即由这三点组成。本德云社票务系统的E-R图如下所示：

1、问题反馈信息实体E-R图如图4-4所示：

![](/md/blog.010.png)

图4-4 问题反馈信息实体的E-R图

2、票务信息实体E-R图如图4-5所示：

![](/md/blog.011.png)

图4-5  票务信息实体E-R图

3、订单实体图如图4-6所示。

![](/md/blog.012.png)

图4-6 订单实体E-R图

4、管理员信息实体图如图4-7所示。

![](/md/blog.013.png)

图4-7 管理员信息实体E-R图

5、会员信息实体图如图4-8所示。

![](/md/blog.014.png)

图4-8  会员信息实体E-R图
### 4.3.2数据库表设计
本德云社票务系统采用了MYSQL数据库进行系统数据的储存，主要的数据库表的具体设置如下：

表4-1 chat问题反馈信息表

|列名|说明|类型 ( 长度 )|备注|
| - | - | - | - |
|id|编号|bigint(20)|不允许空，主键|
|addtime|添加时间|timestamp|允许空|
|userid|用户编号|bigint(20)|允许空|
|adminid|管理员编号|bigint(20)|允许空|
|ask|提问|longtext|允许空|
|reply|回复|longtext|允许空|
|isreply|是否回复|int(11)|允许空|

表4-2  piaowuxinxi票务信息表

|列名|说明|类型 ( 长度 )|备注|
| - | - | - | - |
|id|编号|bigint(20)|不允许空，主键|
|addtime|添加时间|timestamp|允许空|
|piaowumingcheng|票务名称|varchar(200)|允许空|
|piaowutupian|票务图片|varchar(200)|允许空|
|yanchuchengshi|演出城市|varchar(200)|允许空|
|yanchudidian|演出地点|varchar(200)|允许空|
|yanchushijian|演出时间|datetime|允许空|
|jieshushijian|结束时间|datetime|允许空|
|yanchumingdan|演出名单|varchar(200)|允许空|
|zuoweileixing|座位类型|varchar(200)|允许空|
|piaowubeizhu|票务备注|varchar(200)|允许空|
|xuanchuanshipin`|宣传视频|varchar(200)|允许空|
|yanchuxiangqing|演出详情|longtext|允许空|
|clicktime|最近点击时间|datetime|允许空|
|clicknum`|点击次数|int(11)|允许空|
|price`|价格|float|允许空|
|number|座位总数|int(11)|允许空|
|selected`|已选座位|longtext|允许空|

表4-3  orders订单信息表

|列名|说明|类型 ( 长度 )|备注|
| - | - | - | - |
|id|编号|bigint(20)|不允许空，主键|
|addtime|下单时间|timestamp|允许空|
|orderid`|订单编号|varchar(200)|允许空|
|tablename|商品表名|varchar(200)|允许空|
|userid|用户编号|bigint(20)|允许空|
|goodid|商品编号|bigint(20)|允许空|
|goodname|商品名称|varchar(200)|允许空|
|picture|商品图片|varchar(200)|允许空|
|buynumber|购买数量|int(11)|允许空|
|price|价格|float|允许空|
|discountprice|折扣价格|float|允许空|
|total|总价格|float|允许空|
|discounttotal|折扣总价格|float|允许空|
|type|支付类型|int(11)|允许空|
|status|状态|varchar(200)|允许空|
|address|地址|varchar(200)|允许空|

表4-4  users管理员信息表

|列名|说明|类型 ( 长度 )|备注|
| - | - | - | - |
|id|编号|bigint(20)|不允许空，主键|
|username|用户名|varchar(100)|允许空|
|password|密码|varchar(100)|允许空|
|role|角色|varchar(100)|允许空|
|addtime|添加时间|timestamp|允许空|

表4-5  huiyuan会员信息表

|列名|说明|类型 ( 长度 )|备注|
| - | - | - | - |
|id|编号|bigint(20)|不允许空，主键|
|addtime|添加时间|timestamp|允许空|
|yonghuming|用户名|varchar(200)|允许空|
|mima|密码|varchar(200)|允许空|
|xingming|姓名|varchar(200)|允许空|
|touxiang|头像|varchar(200)|允许空|
|xingbie|性别|varchar(200)|允许空|
|shouji|手机|varchar(200)|允许空|
|shenfenzheng|身份证|varchar(200)|允许空|
|money|余额|float|允许空|

#
# 第5章  系统的实现
## 5.1 用户功能模块的实现
用户进入本德云社票务系统可查看票务信息以及公告信息等，系统主界面的运行效果如图5-1所示.

![](/md/blog.015.png)

图5-1系统主界面
### 5.1.1用户登录界面
用户要想实现票务预定操作，必须进行登录操作，在登录界面输入正确的用户名和密码，点击登录按钮进行登录，用户登录界面如图5-2所示。

![](/md/blog.016.png)

图5-2用户登录界面
### 5.1.2用户注册界面
没有账号的用户可进行注册操作，用户注册界面的运行效果如图5-3所示.

![](/md/blog.017.png)

图5-3用户注册界面
### 5.1.3票务详情界面
用户可选择票务查看票务详情信息，登录后可进行收藏以及预定操作，票务详情界面如图5-4所示。

![](/md/blog.018.png)

图5-4  票务详情界面
### 5.1.4票务信息界面
用户在票务信息界面可查看所有票务信息，并可选择查看详情，票务信息界面展示如图5-5所示。

![](/md/blog.019.png)

图5-5  票务信息界面
### 5.1.5我的订单界面
用户可进入我的订单界面查看个人订单信息，我的订单界面如图5-6所示。

![](/md/blog.020.png)

图5-6 我的订单界面
### 5.1.6我的收藏界面
用户在我的收藏界面可查看个人已有收藏信息，我的收藏界面如图5-7所示。

![](/md/blog.021.png)

图5-7  我的收藏界面
## 5.2 管理员功能模块的实现
### 5.2.1管理员登录界面
管理员要想进入系统后台对系统进行管理，首要进入登录界面，需通过正确的账号、密码进行登录操作，管理员登录界面如图5-8所示 。

![](/md/blog.022.png)

图5-8 管理员登录界面
### 5.2.2会员管理界面
管理员在会员管理界面可查看已有会员信息，对已有会员信息管理员可进行修改和删除操作，同时管理员也可进行添加会员信息，会员管理界面展示如图5-9所示 。

![](/md/blog.023.png)

图5-9 会员管理界面
### 5.2.3常见问题管理界面
管理员可添加、修改和删除常见问题信息，常见问题管理界面展示如图5-10所示 。

![](/md/blog.024.png)

图5-10 常见问题管理界面
### 5.2.4票务信息管理界面
管理员可添加、修改和删除票务信息，票务信息管理界面展示如图5-11所示 。添加票务信息界面展示如图5-12所示。

![](/md/blog.025.png)

图5-11票务信息管理界面

![](/md/blog.026.png)

图5-12添加票务信息界面
### 5.2.5订单管理界面
管理员可管理订单信息，包括未支付订单、已支付订单、已完成订单、已取消订单、已退款订单以及已发货订单，其中已支付订单界面如图5-13所示。

![](/md/blog.027.png)

图5-13  已支付订单界面













