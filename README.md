


**最后更新于20180406**

部分内容适用于偏Java方向的架构师，大部分内容适用于所有后端架构师。


# 数据结构

## 队列
* [《java队列——queue详细分析》](https://www.cnblogs.com/lemon-flm/p/7877898.html)
	* 非阻塞队列：ConcurrentLinkedQueue(无界线程安全)，采用CAS机制。
	* 阻塞队列：ArrayBlockingQueue、LinkedBlockingQueue、DelayQueue、PriorityBlockingQueue，采用锁机制。

* [《LinkedList、ConcurrentLinkedQueue、LinkedBlockingQueue对比分析》](https://www.cnblogs.com/mantu/p/5802393.html)

## 集合
* [《Java Set集合的详解》](https://blog.csdn.net/qq_33642117/article/details/52040345)

## 链表、数组
* [《Java集合详解--什么是List》](https://blog.csdn.net/wz249863091/article/details/52853360)

## 字典、关联数组
* [《Java map 详解 - 用法、遍历、排序、常用API等》](https://baike.xsoftlab.net/view/250.html)

## 树

### 二叉树

每个节点最多有两个叶子节点。
*  [《二叉树》](https://blog.csdn.net/cai2016/article/details/52589952)

### 完全二叉树
* [《完全二叉树》](https://baike.baidu.com/item/%E5%AE%8C%E5%85%A8%E4%BA%8C%E5%8F%89%E6%A0%91/7773232?fr=aladdin)
	* 叶节点只能出现在最下层和次下层，并且最下面一层的结点都集中在该层最左边的若干位置的二叉树。

### 平衡二叉树
左右两个子树的高度差的绝对值不超过1，并且左右两个子树都是一棵平衡二叉树。
* [《浅谈数据结构-平衡二叉树》](http://www.cnblogs.com/polly333/p/4798944.html)

### 红黑树
* [《最容易懂得红黑树》](https://blog.csdn.net/sun_tttt/article/details/65445754)
	* 添加阶段后，左旋或者右旋从而再次达到平衡。 

### B-，B+，B*树
MySQL是基于B+树聚集索引组织表

* [《B-树，B+树，B\*树详解》](https://blog.csdn.net/aqzwss/article/details/53074186)
* [《B-树，B+树与B\*树的优缺点比较》](https://blog.csdn.net/bigtree_3721/article/details/73632405)


# 常用算法

* [《常见排序算法及对应的时间复杂度和空间复杂度》](https://blog.csdn.net/gane_cheng/article/details/52652705)

## 排序、查找算法

* [《常见排序算法及对应的时间复杂度和空间复杂度》](https://blog.csdn.net/gane_cheng/article/details/52652705)

### 选择排序
* [《Java中的经典算法之选择排序（SelectionSort）》](https://www.cnblogs.com/shen-hua/p/5424059.html)
	* 每一趟从待排序的记录中选出最小的元素，顺序放在已排好序的序列最后，直到全部记录排序完毕。

### 冒泡排序
* [《冒泡排序的2种写法》](https://blog.csdn.net/shuaizai88/article/details/73250615)
	* 相邻元素前后交换。
	* 时间复杂度 O(n²) 

### 插入排序
* [《排序算法总结之插入排序》](https://blog.csdn.net/shuaizai88/article/details/73250615)

### 快速排序
* [《坐在马桶上看算法：快速排序》](http://developer.51cto.com/art/201403/430986.htm)
	* 一侧比另外一次都大或小。 
### 归并排序
* [《图解排序算法(四)之归并排序》](http://www.cnblogs.com/chengxiao/p/6194356.html)
	* 分而治之，分成小份排序，在合并。 

### 堆排序
* [《图解排序算法(三)之堆排序》](https://www.cnblogs.com/chengxiao/p/6129630.html)
	* 排序过程就是构建最大堆的过程，最大堆：每个结点的值都大于或等于其左右孩子结点的值。

### 计数排序
* [《计数排序和桶排序》](https://www.cnblogs.com/suvllian/p/5495780.html)
	* 和桶排序过程比较像，差别在于桶的数量。

### 桶排序
* [《【啊哈！算法】最快最简单的排序——桶排序》](http://blog.51cto.com/ahalei/1362789)
* [《排序算法（三）：计数排序与桶排序》](https://blog.csdn.net/sunjinshengli/article/details/70738527)
	* 桶排序将[0,1)区间划分为n个相同的大小的子区间，这些子区间被称为桶。
	* 每个通单独进行排序，然后再遍历每个桶。

### 基数排序

按照个位、十位、百位、...依次来排。

* [《排序算法系列：基数排序》](https://blog.csdn.net/u011410529/article/details/56668545?locationnum=6&fps=1)
* [《基数排序》](https://www.cnblogs.com/skywang12345/p/3603669.html)


### 二分查找
* [《二分查找(java实现)》](https://www.cnblogs.com/coderising/p/5708632.html)
	* 要求待查找的序列有序。
	* 时间复杂度 O(logN)。

* [《java实现二分查找-两种方式》](https://blog.csdn.net/maoyuanming0806/article/details/78176957)
	* while + 递归。
### Java 中的排序工具
* [《Arrays.sort和Collections.sort实现原理解析》](https://blog.csdn.net/u011410529/article/details/56668545?locationnum=6&fps=1)
	* 归并排序。

## 贪心算法
* [《算法：贪婪算法基础》](https://www.cnblogs.com/MrSaver/p/8641971.html)
* [《常见算法及问题场景——贪心算法》](https://blog.csdn.net/a345017062/article/details/52443781)

## 回溯算法
* [《 五大常用算法之四：回溯法》](https://blog.csdn.net/qfikh/article/details/51960331)

## 剪枝算法
* [《α-β剪枝算法》](https://blog.csdn.net/luningcsdn/article/details/50930276)

## 动态规划
* [《详解动态规划——邹博讲动态规划》](https://www.cnblogs.com/little-YTMM/p/5372680.html)
* [《动态规划算法的个人理解》](https://blog.csdn.net/yao_zi_jie/article/details/54580283)

## 朴素贝叶斯
* [《贝叶斯推断及其互联网应用》](http://www.ruanyifeng.com/blog/2011/08/bayesian_inference_part_one.html)
* [《贝叶斯推断及其互联网应用》](http://www.ruanyifeng.com/blog/2011/08/bayesian_inference_part_two.html)


## 推荐算法
* [《推荐算法综述》](http://www.infoq.com/cn/articles/recommendation-algorithm-overview-part01)
* [《TOP 10 开源的推荐系统简介》](https://www.oschina.net/news/51297/top-10-open-source-recommendation-systems)


# 并发

## 多线程

* [《40个Java多线程问题总结》](http://www.importnew.com/18459.html)

## 线程安全

* [《Java并发编程——线程安全及解决机制简介》](https://www.cnblogs.com/zhanht/p/5450325.html)

## 一致性、事务

### 事务 ACID 特性
* [《数据库事务ACID特性》](https://blog.csdn.net/u012440687/article/details/52116108)

### 事务的隔离级别

* 未提交读：一个事务可以读取另一个未提交的数据，容易出现脏读的情况。
* 读提交：一个事务等另外一个事务提交之后才可以读取数据，但会出现不可重复读的情况（多次读取的数据不一致），读取过程中出现UPDATE操作，会多。（大多数数据库默认级别是RC，比如SQL Server，Oracle），读取的时候不可以修改。
* 可重复读： 读取的时候就锁定，不可修改（会影响更新），Mysql InnoDB 就是这个级别。
* 序列化：所有事物串行处理（牺牲了效率）


* [《理解事务的4种隔离级别》](https://blog.csdn.net/qq_33290787/article/details/51924963)
* [数据库事务的四大特性及事务隔离级别](https://www.cnblogs.com/z-sm/p/7245981.html)


## 锁

### Java中的锁和同步类

* [《Java中的锁分类》](https://www.cnblogs.com/qifengshi/p/6831055.html)
	* 主要包括 synchronized、ReentrantLock、和 ReadWriteLock。 

* [《Java并发之AQS详解》](https://www.cnblogs.com/waterystone/p/4920797.html)

* [《Java中信号量 Semaphore》](http://cuisuqiang.iteye.com/blog/2020146)
	* 有数量控制
	* 申请用 acquire，申请不要则阻塞；释放用 release。

* [《java开发中的Mutex vs Semaphore》](https://www.cnblogs.com/davidwang456/p/6094947.html)
	* 简单的说 就是Mutex是排它的，只有一个可以获取到资源， Semaphore也具有排它性，但可以定义多个可以获取的资源的对象。	 

### 公平锁 & 非公平锁

公平锁的作用就是严格按照线程启动的顺序来执行的，不允许其他线程插队执行的；而非公平锁是允许插队的。

* [《公平锁与非公平锁》](https://blog.csdn.net/EthanWhite/article/details/55508357)
	* 默认情况下 ReentrantLock 和 synchronized 都是非公平锁。ReentrantLock 可以设置成公平锁。

### 悲观锁 & 乐观锁 & CAS

* [《【MySQL】悲观锁&乐观锁》](https://www.cnblogs.com/zhiqian-ali/p/6200874.html)
	* 乐观锁的方式：版本号+重试方式
	* 悲观锁：通过 select ... for update 进行行锁。

* [《乐观锁的一种实现方式——CAS》](http://www.importnew.com/20472.html)
	* 和MySQL乐观锁方式相似，只不过是通过和原值进行比较。	 

### ABA 问题

由于高并发，在CAS下，更新后可能此A非彼A。通过版本号可以解决，类似于上文Mysql 中提到的的乐观锁。

* [《Java CAS 和ABA问题》](https://www.cnblogs.com/549294286/p/3766717.html)
* [《Java 中 ABA问题及避免》](https://blog.csdn.net/li954644351/article/details/50511879)
	* AtomicStampedReference 和 AtomicStampedReference。 

### CopyOnWrite容器

可以对CopyOnWrite容器进行并发的读，而不需要加锁。CopyOnWrite并发容器用于读多写少的并发场景。比如白名单，黑名单，商品类目的访问和更新场景，不适合需要数据强一致性的场景。

* [《JAVA中写时复制(Copy-On-Write)Map实现》](https://www.cnblogs.com/hapjin/p/4840107.html)
* [《聊聊并发-Java中的Copy-On-Write容器》](https://blog.csdn.net/a494303877/article/details/53404623)

### RingBuffer 
* [《线程安全的无锁RingBuffer的实现【一个读线程，一个写线程】》](http://www.cnblogs.com/l00l/p/4115001.html)

### 可重入锁 & 不可重入锁

* [《可重入锁和不可重入锁》](https://www.cnblogs.com/dj3839/p/6580765.html)
	* 通过简单代码举例说明可重入锁和不可重入锁。
	* 可重入锁指同一个线程可以再次获得之前已经获得的锁。
	* 可重入锁可以用户避免死锁。
	* Java中的可重入锁：synchronized 和  java.util.concurrent.locks.ReentrantLock

* [《ReenTrantLock可重入锁（和synchronized的区别）总结》](https://www.cnblogs.com/baizhanshi/p/7211802.html)
	* synchronized 使用方便，编译器来加锁，是非公平锁。
	* ReenTrantLock 使用灵活，锁的公平性可以定制。
	* 相同加锁场景下，推荐使用 synchronized。





# 操作系统

## 计算机原理

* [《操作系统基础知识——操作系统的原理，类型和结构》](https://segmentfault.com/a/1190000003692840)

## 进程

TODO

## 线程

TODO

## 协程

TODO

## Linux

* [《Linux 命令大全》](http://www.runoob.com/linux/linux-command-manual.html)



# 设计模式

## 23种常见设计模式
* [《设计模式》](http://www.runoob.com/design-pattern/design-pattern-tutorial.html)
* [《23种设计模式全解析》](https://www.cnblogs.com/susanws/p/5510229.html)

## 责任链模式

## MVC
* [《MVC 模式》](http://www.runoob.com/design-pattern/mvc-pattern.html)
	* 模型(model)－视图(view)－控制器(controller) 

## IOC
* [《理解 IOC》](https://www.zhihu.com/question/23277575)
* [《IOC 的理解与解释》](https://www.cnblogs.com/NancyStartOnce/p/6813162.html)
	* 正向控制：传统通过new的方式。反向控制，通过容器注入对象。
	* 作用：用于模块解耦。
	* DI：Dependency Injection，即依赖注入，只关心资源使用，不关心资源来源。

## AOP

* [《轻松理解AOP(面向切面编程)》](https://my.oschina.net/yanquan345/blog/203415)
* [《Spring AOP详解》](https://www.cnblogs.com/hongwz/p/5764917.html)
* [《Spring AOP的实现原理》](http://www.importnew.com/24305.html)
	* Spring AOP使用的动态代理，主要有两种方式：JDK动态代理和CGLIB动态代理。
* [《Spring AOP 实现原理与 CGLIB 应用》](https://www.ibm.com/developerworks/cn/java/j-lo-springaopcglib/)
	* Spring AOP 框架对 AOP 代理类的处理原则是：如果目标对象的实现类实现了接口，Spring AOP 将会采用 JDK 动态代理来生成 AOP 代理类；如果目标对象的实现类没有实现接口，Spring AOP 将会采用 CGLIB 来生成 AOP 代理类 


## UML

* [《UML教程》](https://www.w3cschool.cn/uml_tutorial/)

## 微服务思想
* [《微服务架构设计》](https://www.cnblogs.com/wintersun/p/6219259.html)
### 康威定律
* [《微服务架构的理论基础 - 康威定律》](https://yq.aliyun.com/articles/8611)
	* 定律一：组织沟通方式会通过系统设计表达出来，就是说架构的布局和组织结构会有相似。
	* 定律二：时间再多一件事情也不可能做的完美，但总有时间做完一件事情。一口气吃不成胖子，先搞定能搞定的。
	* 定律三：线型系统和线型组织架构间有潜在的异质同态特性。种瓜得瓜，做独立自治的字系统减少沟通成本。
	* 定律四：大的系统组织总是比小系统更倾向于分解。合久必分，分而治之。

# 运维 & 统计 & 技术支持 

## 常规监控

* [《腾讯业务系统监控的修炼之路》](https://blog.csdn.net/enweitech/article/details/77849205)
	* 监控的方式：主动、被动、旁路(比如舆情监控)
	* 监控类型： 基础监控、服务端监控、客户端监控、WEB监控、用户端监控
	* 监控的目标：全、块、准
	* 核心指标：请求量、成功率、耗时

* [《开源还是商用？十大云运维监控工具横评》](https://www.oschina.net/news/67525/monitoring-tools)
	* Zabbix、Nagios、Ganglia、Zenoss、Open-falcon、监控宝、 360网站服务监控、阿里云监控、百度云观测、小蜜蜂网站监测等。

* [《监控报警系统搭建及二次开发经验》](http://developer.51cto.com/art/201612/525373.htm)

**命令行监控工具**

* [《常用命令行监控工具》](https://coderxing.gitbooks.io/architecture-evolution/di-er-pian-ff1a-feng-kuang-yuan-shi-ren/44-an-quan-yu-yun-wei/445-fu-wu-qi-zhuang-tai-jian-ce/4451-ming-ling-xing-gong-ju.html)
	* top、sar、tsar、nload

* [《20个命令行工具监控 Linux 系统性能》](http://blog.jobbole.com/96846/)

* [《JVM性能调优监控工具jps、jstack、jmap、jhat、jstat、hprof使用详解》](https://my.oschina.net/feichexia/blog/196575)

## APM

APM —  Application Performance Management

* [《Dapper，大规模分布式系统的跟踪系统》](http://bigbully.github.io/Dapper-translation/)

* [《开源APM技术选型与实战》](http://www.infoq.com/cn/articles/apm-Pinpoint-practice)
	* 主要基于 Google的Dapper（大规模分布式系统的跟踪系统） 思想。
	* 开源软件有：Pinpoint、SkyWalking、Zipkin、CAT


## 统计分析

* [《流量统计的基础：埋点》](https://zhuanlan.zhihu.com/p/25195217)
	* 常用指标：访问与访客、停留时长、跳出率、退出率、转化率、参与度

* [《APP埋点常用的统计工具、埋点目标和埋点内容》](http://www.25xt.com/company/17066.html)
	* 第三方统计：友盟、百度移动、魔方、App Annie、talking data、神策数据等。

* [《美团点评前端无痕埋点实践》](https://tech.meituan.com/mt-mobile-analytics-practice.html)
	* 所谓无痕、即通过可视化工具配置采集节点，在前端自动解析配置并上报埋点数据，而非硬编码。 


## 持续集成

* [《持续集成是什么？》](http://www.ruanyifeng.com/blog/2015/09/continuous-integration.html)
* [《8个流行的持续集成工具》](https://www.testwo.com/article/1170)

### Jenkins

* [《使用Jenkins进行持续集成》](https://www.liaoxuefeng.com/article/001463233913442cdb2d1bd1b1b42e3b0b29eb1ba736c5e000)

### 环境分离

开发、测试、生成环境分离。

* [《开发环境、生产环境、测试环境的基本理解和区》](https://my.oschina.net/sancuo/blog/214904)

## 自动化运维

### Ansible
* [《Ansible中文权威指南》](http://www.ansible.com.cn/)
* [《Ansible基础配置和企业级项目实用案例》](https://www.cnblogs.com/heiye123/articles/7855890.html)

### puppet
* [《自动化运维工具——puppet详解》](https://www.cnblogs.com/keerya/p/8040071.html)

### chef
* [《Chef 的安装与使用》](https://www.ibm.com/developerworks/cn/cloud/library/1407_caomd_chef/)

## 测试

### TDD 理论

* [《深度解读 - TDD（测试驱动开发）》](https://www.jianshu.com/p/62f16cd4fef3)
	* 基于测试用例编码功能代码，XP（Extreme Programming）的核心实践.
	* 好处：一次关注一个点，降低思维负担；迎接需求变化或改善代码的设计；提前澄清需求；快速反馈； 

### 单元测试

* [《Java单元测试之JUnit篇》](https://www.cnblogs.com/happyzm/p/6482886.html)
* [《JUnit 4 与 TestNG 对比》](https://blog.csdn.net/hotdust/article/details/53406086)
	* TestNG 覆盖 JUnit 功能，适用于更复杂的场景。 
* [《单元测试主要的测试功能点》](https://blog.csdn.net/wqetfg/article/details/50900512)
	* 模块接口测试、局部数据结构测试、路径测试 、错误处理测试、边界条件测试 。 

### 压力测试

* [《Apache ab 测试使用指南》](https://blog.csdn.net/blueheart20/article/details/52170790)
* [《大型网站压力测试及优化方案》](https://www.cnblogs.com/binyue/p/6141088.html)
* [《10大主流压力/负载/性能测试工具推荐》](http://news.chinabyte.com/466/14126966.shtml)
* [《真实流量压测工具 tcpcopy应用浅析》](http://quentinxxz.iteye.com/blog/2249799)
* [《nGrinder 简易使用教程》](https://www.cnblogs.com/jwentest/p/7136727.html)


### 全链路压测
* [《京东618：升级全链路压测方案，打造军演机器人ForceBot》](http://www.infoq.com/cn/articles/jd-618-upgrade-full-link-voltage-test-program-forcebot)
* [《饿了么全链路压测的探索与实践》](https://zhuanlan.zhihu.com/p/30306892)
* [《四大语言，八大框架｜滴滴全链路压测解决之道》](https://zhuanlan.zhihu.com/p/28355759)
* [《全链路压测经验》](https://www.jianshu.com/p/27060fd61f72)


### A/B Test

* [《技术干货 | AB 测试和灰度发布探索及实践》](https://testerhome.com/topics/11165)
* [《nginx 根据IP 进行灰度发布》](http://blog.51cto.com/purplegrape/1403123)


## 虚拟化

* [《VPS的三种虚拟技术OpenVZ、Xen、KVM优缺点比较》](https://blog.csdn.net/enweitech/article/details/52910082)

### KVM
* [《KVM详解，太详细太深入了，经典》](http://blog.chinaunix.net/uid-20201831-id-5775661.html)
* [《【图文】KVM 虚拟机安装详解》](https://www.coderxing.com/kvm-install.html)

### Xen
* [《Xen虚拟化基本原理详解》](https://www.cnblogs.com/sddai/p/5931201.html)

### OpenVZ
* [《开源Linux容器 OpenVZ 快速上手指南》](https://blog.csdn.net/longerzone/article/details/44829255)

## 容器技术

### Docker
* [《几张图帮你理解 docker 基本原理及快速入门》](https://www.cnblogs.com/SzeCheng/p/6822905.html)
* [《Docker 核心技术与实现原理》](https://draveness.me/docker)
* [《Docker 教程》](http://www.runoob.com/docker/docker-tutorial.html)

## 云技术

### OpenStack
* [《OpenStack构架知识梳理》](https://www.cnblogs.com/klb561/p/8660264.html)

## DevOps
* [《一分钟告诉你究竟DevOps是什么鬼？》](https://www.cnblogs.com/jetzhang/p/6068773.html)
* [《DevOps详解》](http://www.infoq.com/cn/articles/detail-analysis-of-devops)

## 文档管理

* [Confluence-收费文档管理系统](http://www.confluence.cn/)
* GitLab?
* Wiki

# 中间件

## Web Server

### Nginx
* [《Ngnix的基本学习-多进程和Apache的比较》](https://blog.csdn.net/qq_25797077/article/details/52200722)
	* Nginx 通过异步非阻塞的事件处理机制实现高并发。Apache 每个请求独占一个线程，非常消耗系统资源。
	* 事件驱动适合于IO密集型服务(Nginx)，多进程或线程适合于CPU密集型服务(Apache)，所以Nginx适合做反向代理，而非web服务器使用。  

* [《nginx与Apache的对比以及优缺点》](https://www.cnblogs.com/cunkouzh/p/5410154.html)
	* nginx只适合静态和反向代理，不适合处理动态请求。

### OpenResty
* [官方网站](http://openresty.org/cn/)
* [《浅谈 OpenResty》](http://www.linkedkeeper.com/detail/blog.action?bid=1034)
	* 通过 Lua 模块可以在Nginx上进行开发。 

### Apache Httpd
* [官方网站](http://httpd.apache.org/)

### Tomcat

* [《TOMCAT原理详解及请求过程》](https://www.cnblogs.com/hggen/p/6264475.html)
* [《Tomcat服务器原理详解》](https://www.cnblogs.com/crazylqy/p/4706223.html)
* [《Tomcat 系统架构与设计模式,第 1 部分: 工作原理》](https://www.ibm.com/developerworks/cn/java/j-lo-tomcat1/)

* [《JBoss vs. Tomcat: Choosing A Java Application Server》](https://www.futurehosting.com/blog/jboss-vs-tomcat-choosing-a-java-application-server/)
	* Tomcat 是轻量级的 Serverlet 容器，没有实现全部 JEE 特性（比如持久化和事务处理），但可以通过其他组件代替，比如Srping。
	* Jboss 实现全部了JEE特性，软件开源免费、文档收费。

* [《Tomcat 调优方案》](https://www.cnblogs.com/sunfenqing/p/7339058.html)
	* 启动NIO模式（或者APR）；调整线程池；禁用AJP连接器（Nginx+tomcat的架构，不需要AJP）； 

* [《tomcat http协议与ajp协议》](http://blog.chinaunix.net/uid-20662363-id-3012760.html)
* [《AJP与HTTP比较和分析》](http://dmouse.iteye.com/blog/1354527)
	* AJP 协议（8009端口）用于降低和前端Server（如Apache，而且需要支持AJP协议）的连接数(前端)，通过长连接提高性能。
	* 并发高时，AJP协议优于HTTP协议。

### Jetty
* [《Jetty 的工作原理以及与 Tomcat 的比较》](https://www.ibm.com/developerworks/cn/java/j-lo-jetty/)
* [《jetty和tomcat优势比较》](https://blog.csdn.net/doutao6677/article/details/51957288)
	* 架构比较:Jetty的架构比Tomcat的更为简单。
	* 性能比较：Jetty和Tomcat性能方面差异不大，Jetty默认采用NIO结束在处理I/O请求上更占优势，Tomcat默认采用BIO处理I/O请求，Tomcat适合处理少数非常繁忙的链接，处理静态资源时性能较差。
	* 其他方面：Jetty的应用更加快速，修改简单，对新的Servlet规范的支持较好;Tomcat 对JEE和Servlet 支持更加全面。 



## 缓存

* [《缓存失效策略（FIFO 、LRU、LFU三种算法的区别）》](https://blog.csdn.net/clementad/article/details/48229243)

### 本地缓存

* [《HashMap本地缓存》](https://coderxing.gitbooks.io/architecture-evolution/di-er-pian-ff1a-feng-kuang-yuan-shi-ren/42-xing-neng-zhi-ben-di-huan-cun/421-ying-yong-ceng-ben-di-huan-cun/4211.html)

* [《EhCache本地缓存》](https://coderxing.gitbooks.io/architecture-evolution/di-er-pian-ff1a-feng-kuang-yuan-shi-ren/42-xing-neng-zhi-ben-di-huan-cun/421-ying-yong-ceng-ben-di-huan-cun/4212-ehcache.html)
	* 堆内、堆外、磁盘三级缓存。
	* 可按照缓存空间容量进行设置。
	* 按照时间、次数等过期策略。

* [《Guava Cache》](https://coderxing.gitbooks.io/architecture-evolution/di-er-pian-ff1a-feng-kuang-yuan-shi-ren/42-xing-neng-zhi-ben-di-huan-cun/421-ying-yong-ceng-ben-di-huan-cun/4213-guava-cache.html)
	* 简单轻量、无堆外、磁盘缓存。

* [《Guava Cache》](https://coderxing.gitbooks.io/architecture-evolution/di-er-pian-ff1a-feng-kuang-yuan-shi-ren/42-xing-neng-zhi-ben-di-huan-cun/421-ying-yong-ceng-ben-di-huan-cun/4213-guava-cache.html)
	* 简单轻量、无堆外、磁盘缓存。

* [《Nginx本地缓存》](https://coderxing.gitbooks.io/architecture-evolution/di-er-pian-ff1a-feng-kuang-yuan-shi-ren/42-xing-neng-zhi-ben-di-huan-cun/422-fu-wu-duan-ben-di-huan-cun/nginx-ben-di-huan-cun.html)

* [《Pagespeed—懒人工具，服务器端加速》](https://coderxing.gitbooks.io/architecture-evolution/di-er-pian-ff1a-feng-kuang-yuan-shi-ren/42-xing-neng-zhi-ben-di-huan-cun/422-fu-wu-duan-ben-di-huan-cun/4222-pagespeed.html)

## 客户端缓存

* [《浏览器端缓存》](https://coderxing.gitbooks.io/architecture-evolution/di-er-pian-ff1a-feng-kuang-yuan-shi-ren/42-xing-neng-zhi-ben-di-huan-cun/423-ke-hu-duan-huan-cun.html)
	* 主要是利用 Cache-Control 参数。

* [《H5 和移动端 WebView 缓存机制解析与实战》](https://mp.weixin.qq.com/s/qHm_dJBhVbv0pJs8Crp77w)

### Memcached
* [《Memcached 教程》](http://www.runoob.com/Memcached/Memcached-tutorial.html)
* [《深入理解Memcached原理》](https://blog.csdn.net/chenleixing/article/details/47035453)
	* 采用多路复用技术提高并发性。
	* slab分配算法： memcached给Slab分配内存空间，默认是1MB。分配给Slab之后 把slab的切分成大小相同的chunk，Chunk是用于缓存记录的内存空间，Chunk 的大小默认按照1.25倍的速度递增。好处是不会频繁申请内存，提高IO效率，坏处是会有一定的内存浪费。
* [《Memcached软件工作原理》](https://www.jianshu.com/p/36e5cd400580)
* [《Memcache技术分享：介绍、使用、存储、算法、优化、命中率》](http://zhihuzeye.com/archives/2361)


* [**《memcached全面剖析》**](https://pan.baidu.com/s/1qX00Lti?errno=0&errmsg=Auth%20Login%20Sucess&&bduss=&ssnerror=0&traceid=)

### Redis
* [《Redis 教程》](http://www.runoob.com/redis/redis-tutorial.html)
* [《redis底层原理》](https://blog.csdn.net/wcf373722432/article/details/78678504)
	* 使用 ziplist 存储链表，ziplist是一种压缩链表，它的好处是更能节省内存空间，因为它所存储的内容都是在连续的内存区域当中的。
	* 使用 skiplist(跳跃表)来存储有序集合对象、查找上先从高Level查起、时间复杂度和红黑树相当，实现容易，无锁、并发性好。
* [《Redis持久化方式》](http://doc.redisfans.com/topic/persistence.html)
	* RDB方式：定期备份快照，常用于灾难恢复。优点：通过fork出的进程进行备份，不影响主进程、RDB 在恢复大数据集时的速度比 AOF 的恢复速度要快。缺点：会丢数据。
	* AOF方式：保存操作日志方式。优点：恢复时数据丢失少，缺点：文件大，回复慢。
	* 也可以两者结合使用。

### Tair

* [官方网站](https://github.com/alibaba/tair)
* [《Tair和Redis的对比》](http://blog.csdn.net/farphone/article/details/53522383)
* ​
* 特点：可以配置备份节点数目，通过异步同步到备份节点
* 一致性Hash算法。
* 架构：和Hadoop 的设计思想类似，有Configserver，DataServer，Configserver 通过心跳来检测，Configserver也有主备关系。


几种存储引擎:
* MDB，完全内存性，可以用来存储Session等数据。
* Rdb（类似于Redis），轻量化，去除了aof之类的操作，支持Restfull操作
* LDB（LevelDB存储引擎），持久化存储，LDB 作为rdb的持久化，google实现，比较高效，理论基础是LSM(Log-Structured-Merge Tree)算法，现在内存中修改数据，达到一定量时（和内存汇总的旧数据一同写入磁盘）再写入磁盘，存储更加高效，县比喻Hash算法。
* Tair采用共享内存来存储数据，如果服务挂掉（非服务器），重启服务之后，数据亦然还在。

## 消息队列

* [《消息队列-推/拉模式学习 & ActiveMQ及JMS学习》](https://www.cnblogs.com/charlesblc/p/6045238.html)
	* RabbitMQ 消费者默认是推模式（也支持拉模式）。
	* Kafka 默认是拉模式。
	* Push方式：优点是可以尽可能快地将消息发送给消费者，缺点是如果消费者处理能力跟不上，消费者的缓冲区可能会溢出。
	* Pull方式：优点是消费端可以按处理能力进行拉去，缺点是会增加消息延迟。

* [《Kafka、RabbitMQ、RocketMQ等消息中间件的对比 —— 消息发送性能和区别》](https://blog.csdn.net/yunfeng482/article/details/72856762)

### 消息总线

消息总线相当于在消息队列之上做了一层封装，统一入口，统一管控、简化接入成本。

* [《消息总线VS消息队列》](https://blog.csdn.net/yanghua_kobe/article/details/43877281)


### RabbitMQ

支持事务，推拉模式都是支持、适合需要可靠性消息传输的场景。

* [《RabbitMQ的应用场景以及基本原理介绍》](https://blog.csdn.net/whoamiyang/article/details/54954780)
* [《消息队列之 RabbitMQ》](https://www.jianshu.com/p/79ca08116d57) 
* [《RabbitMQ之消息确认机制（事务+Confirm）》](https://blog.csdn.net/u013256816/article/details/55515234)

### RocketMQ
Java实现，推拉模式都是支持，吞吐量逊于Kafka。可以保证消息顺序。
* [《RocketMQ 实战之快速入门》](https://www.jianshu.com/p/824066d70da8)

### ActiveMQ
纯Java实现，兼容JMS，可以内嵌于Java应用中。
* [《ActiveMQ消息队列介绍》](https://www.cnblogs.com/wintersun/p/3962302.html)

### Kafka
高吞吐量、采用拉模式。适合搞IO场景，比如日志同步。

* [官方网站](http://kafka.apache.org/)
* [《各消息队列对比，Kafka深度解析，众人推荐，精彩好文！》](https://blog.csdn.net/allthesametome/article/details/47362451)
* [《Kafka分区机制介绍与示例》](http://lxw1234.com/archives/2015/10/538.htm)

### Redis 消息推送

生产者、消费者模式完全是客户端行为，list 和 拉模式实现，阻塞等待采用 blpop 指令。

* [《Redis学习笔记之十：Redis用作消息队列》](https://blog.csdn.net/qq_34212276/article/details/78455004)

### ZeroMQ
 TODO


## 定时调度

### 单机定时调度

* [《linux定时任务cron配置》](https://www.cnblogs.com/shuaiqing/p/7742382.html)

* [《Linux cron运行原理》](https://my.oschina.net/daquan/blog/483305)
	* fork 进程 + sleep 轮询

* [《Quartz使用总结》](https://www.cnblogs.com/drift-ice/p/3817269.html)
* [《Quartz源码解析 ---- 触发器按时启动原理》](https://blog.csdn.net/wenniuwuren/article/details/42082981/)
* [《quartz原理揭秘和源码解读》](https://www.jianshu.com/p/bab8e4e32952)
	* 定时调度在 QuartzSchedulerThread 代码中，while()无限循环，每次循环取出时间将到的trigger，触发对应的job，直到调度器线程被关闭。


### 分布式定时调度

* [《这些优秀的国产分布式任务调度系统，你用过几个？》](https://blog.csdn.net/qq_16216221/article/details/70314337)
	* opencron、LTS、XXL-JOB、Elastic-Job、Uncode-Schedule、Antares

* [《Quartz任务调度的基本实现原理》](https://www.cnblogs.com/zhenyuyaodidiao/p/4755649.html)
	* Quartz集群中，独立的Quartz节点并不与另一其的节点或是管理节点通信，而是通过相同的数据库表来感知到另一Quartz应用的 


## RPC

* [《从零开始实现RPC框架 - RPC原理及实现》](https://blog.csdn.net/top_code/article/details/54615853)
	* 核心角色：Server: 暴露服务的服务提供方、Client: 调用远程服务的服务消费方、Registry: 服务注册与发现的注册中心。

* [《分布式RPC框架性能大比拼 dubbo、motan、rpcx、gRPC、thrift的性能比较》](https://blog.csdn.net/testcs_dn/article/details/78050590)

### Dubbo
* [官方网站](http://dubbo.apache.org/)
* [dubbo实现原理简单介绍](https://www.cnblogs.com/steven520213/p/7606598.html)

### Thrift
* [官方网站](http://thrift.apache.org/)
* [《Thrift RPC详解》](https://blog.csdn.net/kesonyk/article/details/50924489)
	* 支持多语言，通过中间语言定义接口。

### gRPC

服务端可以认证加密，在外网环境下，可以保证数据安全。

* [官方网站](https://grpc.io/)
* [《你应该知道的RPC原理》](https://www.cnblogs.com/LBSer/p/4853234.html)


## 数据库中间件

### Sharding Jdbc

* [官网](http://shardingjdbc.io/)

## 日志系统

### 日志搜集

* [《从零开始搭建一个ELKB日志收集系统》](http://cjting.me/misc/build-log-system-with-elkb/)
* [《用ELK搭建简单的日志收集分析系统》](https://blog.csdn.net/lzw_2006/article/details/51280058)
* [《日志收集系统-探究》](https://www.cnblogs.com/beginmind/p/6058194.html)

## 配置中心

* [Apollo - 携程开源的配置中心应用](https://github.com/ctripcorp/apollo)
	* Spring Boot 和 Spring Cloud
	* 支持推、拉模式更新配置
	* 支持多种语言 

* [《基于zookeeper实现统一配置管理》](https://blog.csdn.net/u011320740/article/details/78742625)

* [《 Spring Cloud Config 分布式配置中心使用教程》](https://www.cnblogs.com/shamo89/p/8016908.html)

servlet 3.0 异步特性可用于配置中心的客户端
* [《servlet3.0 新特性——异步处理》](https://www.cnblogs.com/dogdogwang/p/7151866.html)

## API 网关

主要职责：请求转发、安全认证、协议转换、容灾。

* [《API网关那些儿》](http://yunlzheng.github.io/2017/03/14/the-things-about-api-gateway/)
* [《谈API网关的背景、架构以及落地方案》](http://www.infoq.com/cn/news/2016/07/API-background-architecture-floo)

* [《使用Zuul构建API Gateway》](https://blog.csdn.net/zhanglh046/article/details/78651993)
* [《HTTP API网关选择之一Kong介绍》](https://mp.weixin.qq.com/s/LIq2CiXJQmmjBC0yvYLY5A)

# 网络


## 协议
### TCP/IP
* [《深入浅出 TCP/IP 协议》](https://www.cnblogs.com/onepixel/p/7092302.html)

### HTTP
* [《http协议详解(超详细)》](https://www.cnblogs.com/wangning528/p/6388464.html)

### HTTP2.0
* [《HTTP 2.0 原理详细分析》](https://blog.csdn.net/zhuyiquan/article/details/69257126)

### HTTPS
* [《https原理通俗了解》](https://www.cnblogs.com/zhangshitong/p/6478721.html)
* [《八大免费SSL证书-给你的网站免费添加Https安全加密》](https://blog.csdn.net/enweitech/article/details/53213862)

## 网络模型

* [《web优化必须了解的原理之I/o的五种模型和web的三种工作模式》](http://blog.51cto.com/litaotao/1289790)
	* 五种I/O模型：阻塞I/O，非阻塞I/O，I/O复用、事件(信号)驱动I/O、异步I/O，前四种I/O属于同步操作，I/O的第一阶段不同、第二阶段相同，最后的一种则属于异步操作。
	* 三种 Web Server 工作方式：Prefork(多进程)、Worker方式(线程方式)、Event方式。

* [《select、poll、epoll之间的区别总结》](http://www.cnblogs.com/Anker/p/3265058.html)
	* select，poll，epoll本质上都是同步I/O，因为他们都需要在读写事件就绪后自己负责进行读写，也就是说这个读写过程是阻塞的。
	* select 有打开文件描述符数量限制，默认1024（2048 for x64），100万并发，就要用1000个进程、切换开销大；poll采用链表结构，没有数量限制。
	* select，poll “醒着”的时候要遍历整个fd集合，而epoll在“醒着”的时候只要判断一下就绪链表是否为空就行了，通过回调机制节省大量CPU时间；select，poll每次调用都要把fd集合从用户态往内核态拷贝一次，而epoll只要一次拷贝。
	* poll会随着并发增加，性能逐渐下降，epoll采用红黑树结构，性能稳定，不会随着连接数增加而降低。
	
* [《select，poll，epoll比较  》](http://xingyunbaijunwei.blog.163.com/blog/static/76538067201241685556302/)
	* 在连接数少并且连接都十分活跃的情况下，select和poll的性能可能比epoll好，毕竟epoll的通知机制需要很多函数回调。

* [《深入理解Java NIO》](https://www.cnblogs.com/geason/p/5774096.html)
	* NIO 是一种同步非阻塞的 IO 模型。同步是指线程不断轮询 IO 事件是否就绪，非阻塞是指线程在等待 IO 的时候，可以同时做其他任务

* [《BIO与NIO、AIO的区别》](https://blog.csdn.net/skiof007/article/details/52873421)

* [《两种高效的服务器设计模型：Reactor和Proactor模型》](https://blog.csdn.net/u013074465/article/details/46276967)

### Epoll

* [《epoll使用详解（精髓）》](https://www.cnblogs.com/fnlingnzb-learner/p/5835573.html)

### NIO
* [《深入理解Java NIO》](https://www.cnblogs.com/geason/p/5774096.html)

### kqueue
* [《kqueue用法简介》](http://www.cnblogs.com/luminocean/p/5631336.html)

## 框架

* [《Netty原理剖析》](https://blog.csdn.net/excellentyuxiao/article/details/53390408)
	* Reactor 模式介绍。
	* Netty 是 Reactor 模式的一种实现。


## 序列化(二进制协议)

### Hessian
* [《Hessian原理分析》](https://www.cnblogs.com/happyday56/p/4268249.html)
Binary-RPC;不仅仅是序列化

### Protobuf
* [《Protobuf协议的Java应用例子》](https://blog.csdn.net/antgan/article/details/52103966)
Goolge出品、占用空间和效率完胜其他序列化类库，如Hessian；需要编写  .proto 文件。
* [《Protocol Buffers序列化协议及应用》](https://worktile.com/tech/share/prototol-buffers)
  关于协议的解释；缺点：可读性差;


#数据库

## MySQL

### 原理
* [《MySQL的InnoDB索引原理详解》] (http://www.admin10000.com/document/5372.html)

* [《MySQL存储引擎－－MyISAM与InnoDB区别》](https://blog.csdn.net/xifeijian/article/details/20316775)
	* 两种类型最主要的差别就是Innodb 支持事务处理与外键和行级锁

* [《myisam和innodb索引实现的不同》](https://www.2cto.com/database/201211/172380.html)

### 优化

* [《MYSQL性能优化的最佳20+条经验》](https://www.cnblogs.com/zhouyusheng/p/8038224.html)


## NoSQL

### MongoDB

* [MongoDB 教程](http://www.runoob.com/mongodb/mongodb-tutorial.html)
* [《Mongodb相对于关系型数据库的优缺点》](http://mxdxm.iteye.com/blog/2093603)
	* 优点：弱一致性（最终一致），更能保证用户的访问速度；内置GridFS，支持大容量的存储；Schema-less 数据库，不用预先定义结构；内置Sharding；相比于其他NoSQL，第三方支持丰富；性能优越；
	* 缺点：mongodb不支持事务操作；mongodb占用空间过大；MongoDB没有如MySQL那样成熟的维护工具，这对于开发和IT运营都是个值得注意的地方；

### Hbase

* [《简明 HBase 入门教程（开篇）》](http://www.thebigdata.cn/HBase/35831.html)
* [《深入学习HBase架构原理》](https://www.cnblogs.com/qiaoyihang/p/6246424.html)
* [《传统的行存储和（HBase）列存储的区别》](https://blog.csdn.net/youzhouliu/article/details/67632882)



# 搜索引擎

## 搜索引擎原理

* [《倒排索引--搜索引擎入门》](https://www.jianshu.com/p/0193dc44135b)

## Lucene
* [《Lucene入门简介》](https://www.cnblogs.com/rodge-run/p/6551152.html)

## Elasticsearch

* [《Elasticsearch学习，请先看这一篇！》](https://blog.csdn.net/laoyang360/article/details/52244917)
* [《Elasticsearch索引原理》](https://blog.csdn.net/cyony/article/details/65437708)

## Solr
* [《 Apache Solr入门教程》](https://blog.csdn.net/u011936655/article/details/51960005)
* [《elasticsearch与solr比较》](https://blog.csdn.net/convict_eva/article/details/53537837)

## sphinx 
* [《Sphinx 的介绍和原理探索》](http://blog.jobbole.com/101672/)

# 性能

## 性能优化方法论

* [《15天的性能优化工作，5方面的调优经验》](https://blog.csdn.net/huangwenyi1010/article/details/72673447?ref=myread)
	* 代码层面、业务层面、数据库层面、服务器层面、前端优化。

* [《系统性能优化的几个方面》](https://blog.csdn.net/tenglizhe/article/details/44563135)

## 容量评估
* [《联网性能与容量评估的方法论和典型案例》](https://blog.csdn.net/u012528360/article/details/70054156)

## CDN 网络

* [《CDN加速原理》](https://www.cnblogs.com/wxiaona/p/5867685.html)
* [《国内有哪些比较好的 CDN？》](https://www.zhihu.com/question/20536932)

## 连接池

* [《主流Java数据库连接池比较与开发配置实战》](https://blog.csdn.net/fysuccess/article/details/66972554)

## 性能调优

* [《九大Java性能调试工具，必备至少一款》](https://blog.csdn.net/yethyeth/article/details/73266455)


#大数据

## 流式计算

### Storm
* [官方网站](http://storm.apache.org/)
* [《最详细的Storm入门教程》](https://blog.csdn.net/uisoul/article/details/77989927)

### Flink
* [《Flink之一 Flink基本原理介绍》](https://blog.csdn.net/lisi1129/article/details/54844919)

### Kafka Stream
* [《Kafka Stream调研：一种轻量级流计算模式》](https://yq.aliyun.com/articles/58382)

### 应用场景

例如：

* 广告相关实时统计；
* 推荐系统用户画像标签实时更新；
* 线上服务健康状况实时监测；
* 实时榜单；
* 实时数据统计。

## Hadoop

* [《用通俗易懂的话说下hadoop是什么,能做什么》](https://blog.csdn.net/houbin0912/article/details/72967178)
* [《史上最详细的Hadoop环境搭建》](http://gitbook.cn/books/5954c9600326c7705af8a92a/index.html)

### HDFS
* [《【Hadoop学习】HDFS基本原理》](https://segmentfault.com/a/1190000011575458)

### MapReduce
* [《用通俗易懂的大白话讲解Map/Reduce原理》](https://blog.csdn.net/oppo62258801/article/details/72884633)
* [《 简单的map-reduce的java例子》](https://blog.csdn.net/foye12/article/details/78358292)

### Yarn
* [《初步掌握Yarn的架构及原理》](http://www.cnblogs.com/codeOfLife/p/5492740.html)

## Spark
* [《Spark(一): 基本架构及原理》](http://www.cnblogs.com/tgzhu/p/5818374.html)


# 安全

## web 安全

### XSS
* [《xss攻击原理与解决方法》](https://blog.csdn.net/qq_21956483/article/details/54377947)
### CSRF
* [《CSRF原理及防范》](https://coderxing.gitbooks.io/architecture-evolution/di-san-pian-ff1a-bu-luo/641-web-an-quan-fang-fan/6412-csrf.html)

### SQL 注入

* [《SQL注入》](https://coderxing.gitbooks.io/architecture-evolution/di-san-pian-ff1a-bu-luo/641-web-an-quan-fang-fan/6413-sql-zhu-ru.html)

### 脚本注入

* [《上传文件漏洞原理及防范》](https://coderxing.gitbooks.io/architecture-evolution/di-san-pian-ff1a-bu-luo/641-web-an-quan-fang-fan/6414-shang-chuan-wen-jian-guo-lv.html)

### 漏洞扫描工具
* [《DVWA》](https://coderxing.gitbooks.io/architecture-evolution/di-san-pian-ff1a-bu-luo/6421-dvwa.html)
* [W3af](https://coderxing.gitbooks.io/architecture-evolution/di-san-pian-ff1a-bu-luo/w3af.html)
* [OpenVAS详解](https://blog.csdn.net/xygg0801/article/details/53610640)

### 验证码

* [《验证码原理分析及实现》](https://blog.csdn.net/niaonao/article/details/51112686)

* [《详解滑动验证码的实现原理》](https://my.oschina.net/jiangbianwanghai/blog/1031031)
	* 滑动验证码是根据人在滑动滑块的响应时间，拖拽速度，时间，位置，轨迹，重试次数等来评估风险。

* [《淘宝滑动验证码研究》](https://www.cnblogs.com/xcj26/p/5242758.html)

## DDoS 防范
* [《学习手册：DDoS的攻击方式及防御手段》](http://netsecurity.51cto.com/art/201601/503799.htm)
* [《免费DDoS攻击测试工具大合集》](http://netsecurity.51cto.com/art/201406/442756.htm)

## 加密解密

### 对称加密

* [《常见对称加密算法》](https://coderxing.gitbooks.io/architecture-evolution/di-san-pian-ff1a-bu-luo/642-shu-ju-jia-mi/6421-chang-jian-dui-cheng-jia-mi-suan-fa.html)
	* DES、3DES、Blowfish、AES
	* DES 采用 56位秘钥，Blowfish 采用1到448位变长秘钥，AES 128，192和256位长度的秘钥。
	* DES 秘钥太短（只有56位）算法目前已经被 AES 取代，并且 AES 有硬件加速，性能很好。
	
### 哈希算法
* [《常用的哈希算法》](https://coderxing.gitbooks.io/architecture-evolution/di-san-pian-ff1a-bu-luo/642-shu-ju-jia-mi/6422-chang-jian-ha-xi-suan-fa-and-hmac.html)
	* MD5 和 SHA-1 已经不再安全，已被弃用。
	* 目前 SHA-256 是比较安全的。
	
* [《基于Hash摘要签名的公网URL签名验证设计方案》](https://blog.csdn.net/zhangruhong168/article/details/78033202)

### 非对称加密
* [《常见非对称加密算法》](https://coderxing.gitbooks.io/architecture-evolution/di-san-pian-ff1a-bu-luo/642-shu-ju-jia-mi/6424-chang-yong-fei-dui-cheng-jia-mi-suan-fa.html)
	* RSA、DSA、ECDSA(螺旋曲线加密算法)
	* 和 RSA 不同的是 DSA 仅能用于数字签名，不能进行数据加密解密，其安全性和RSA相当，但其性能要比RSA快。
	* 256位的ECC秘钥的安全性等同于3072位的RSA秘钥。

		[《区块链的加密技术》](http://baijiahao.baidu.com/s?id=1578348858092033763&wfr=spider&for=pc)	


## 服务器安全
* [《Linux强化论：15步打造一个安全的Linux服务器》](http://www.freebuf.com/articles/system/121540.html)

## 数据安全

### 数据备份

TODO

## 网络隔离

### 内外网分离

TODO

### 登录跳板机
在内外环境中通过跳板机登录到线上主机。
* [《搭建简易堡垒机》](http://blog.51cto.com/zero01/2062618)

## 授权
### RBAC 
* [《基于组织角色的权限设计》](https://www.cnblogs.com/zq8024/p/5003050.html)
* [《权限系统与RBAC模型概述》](https://www.cnblogs.com/shijiaqi1066/p/3793894.html)
* [《Spring整合Shiro做权限控制模块详细案例分析》](https://blog.csdn.net/he90227/article/details/38663553)

### OAuth2.0
* [《理解OAuth 2.0》](http://www.ruanyifeng.com/blog/2014/05/oauth_2_0.html)

# 常用开源框架

## 开源协议

* [《开原协议的选择》](https://coderxing.gitbooks.io/architecture-evolution/chapter1/di-yi-zhang-ff1a-zhun-bei-qi-cheng/12-guan-yu-kai-yuan/123-kai-yuan-xie-yi-de-xuan-ze.html)

## 日志框架

### Log4j、Log4j2
* [《log4j 详细讲解》](https://blog.csdn.net/u012422446/article/details/51199724)
* [《log4j2 实际使用详解》](https://blog.csdn.net/vbirdbest/article/details/71751835)
* [《Log4j1,Logback以及Log4j2性能测试对比》](https://my.oschina.net/OutOfMemory/blog/789267)
	* Log4J 异步日志性能优异。 

### Logback
* [《最全LogBack 详解、含java案例和配置说明》](https://blog.csdn.net/rulon147/article/details/52620541)

## ORM

* [《ORM框架使用优缺点》](https://blog.csdn.net/sinat_34093604/article/details/53082000)
	* 主要目的是为了提高开发效率。 

**MyBatis：**

* [《mybatis缓存机制详解》](https://www.cnblogs.com/winclpt/articles/7511672.html)
	* 一级缓存是SqlSession级别的缓存，缓存的数据只在SqlSession内有效
	* 二级缓存是mapper级别的缓存，同一个namespace公用这一个缓存，所以对SqlSession是共享的；使用 LRU 机制清理缓存，通过 cacheEnabled 参数开启。  

* [《MyBatis学习之代码生成器Generator》](https://blog.csdn.net/baidu_32877851/article/details/53959268)

## 网络框架

TODO

## Web 框架

TODO

## 工具框架

* [《Apache Commons 工具类介绍及简单使用》](https://www.cnblogs.com/crazylqy/p/4872236.html)
* [《Google guava 中文教程》](http://ifeve.com/google-guava/)


# 分布式设计

## 扩展性设计

* [《架构师不可不知的十大可扩展架构》](https://blog.csdn.net/hemin1003/article/details/53633926)
	* 总结下来，通用的套路就是分布、缓存及异步处理。 

* [《可扩展性设计之数据切分》](https://yq.aliyun.com/articles/38119)
	* 水平切分+垂直切分
	* 利用中间件进行分片如，MySQL Proxy。
	* 利用分片策略进行切分，如按照ID取模。 
* [《说说如何实现可扩展性的大型网站架构》](https://blog.csdn.net/deniro_li/article/details/78458306)
	* 分布式服务+消息队列。

* [《大型网站技术架构（七）--网站的可扩展性架构》](https://blog.csdn.net/chaofanwei/article/details/29191073)

## 稳定性 & 高可用

* [《系统设计：关于高可用系统的一些技术方案》](https://blog.csdn.net/hustspy1990/article/details/78008324)
	* 可扩展：水平扩展、垂直扩展。 通过冗余部署，避免单点故障。
	* 隔离：避免单一业务占用全部资源。避免业务之间的相互影响 2. 机房隔离避免单点故障。
	* 解耦：降低维护成本，降低耦合风险。减少依赖，减少相互间的影响。
	* 限流：滑动窗口计数法、漏桶算法、令牌桶算法等算法。遇到突发流量时，保证系统稳定。
	* 降级：紧急情况下释放非核心功能的资源。牺牲非核心业务，保证核心业务的高可用。
	* 熔断：异常情况超出阈值进入熔断状态，快速失败。减少不稳定的外部依赖对核心服务的影响。
	* 自动化测试：通过完善的测试，减少发布引起的故障。
	* 灰度发布：灰度发布是速度与安全性作为妥协，能够有效减少发布故障。


* [《关于高可用的系统》](https://coolshell.cn/articles/17459.html)
	* 设计原则：数据不丢(持久化)；服务高可用(服务副本)；绝对的100%高可用很难，目标是做到尽可能多的9，如99.999%（全年累计只有5分钟）。	 

### 硬件负载均衡

* [《转！！负载均衡器技术Nginx和F5的优缺点对比》](https://www.cnblogs.com/wuyun-blog/p/6186198.html)
	* 主要是和F5对比。

* [《软/硬件负载均衡产品 你知多少？》](https://www.cnblogs.com/lcword/p/5773296.html)

### 软件负载均衡

* [《几种负载均衡算法》](https://www.cnblogs.com/tianzhiliang/articles/2317808.html)
	轮寻、权重、负载、最少连接、QoS
* [《DNS负载均衡》](https://coderxing.gitbooks.io/architecture-evolution/di-san-pian-ff1a-bu-luo/611-dns-fang-shi.html)
	* 配置简单，更新速度慢。 
* [《Nginx负载均衡》](https://coderxing.gitbooks.io/architecture-evolution/di-san-pian-ff1a-bu-luo/613-nginx-fu-zai-jun-heng.html)
	* 简单轻量、学习成本低；主要适用于web应用。

*  [《借助LVS+Keepalived实现负载均衡 》](https://www.cnblogs.com/edisonchou/p/4281978.html)
	* 配置比较负载、只支持到4层，性能较高。

* [《HAProxy用法详解 全网最详细中文文档》](http://www.ttlsa.com/linux/haproxy-study-tutorial/)
	* 支持到七层（比如HTTP）、功能比较全面，性能也不错。

* [《Haproxy+Keepalived+MySQL实现读均衡负载》](http://blog.itpub.net/25704976/viewspace-1319781/)
	* 主要是用户读请求的负载均衡。

* [《rabbitmq+haproxy+keepalived实现高可用集群搭建》](https://www.cnblogs.com/lylife/p/5584019.html)

### 限流

* [《谈谈高并发系统的限流》](https://www.cnblogs.com/haoxinyue/p/6792309.html)
	* 计数器：通过滑动窗口计数器，控制单位时间内的请求次数，简单粗暴。
	* 漏桶算法：固定容量的漏桶，漏桶满了就丢弃请求，比较常用。
	* 令牌桶算法：固定容量的令牌桶，按照一定速率添加令牌，处理请求前需要拿到令牌，拿不到令牌则丢弃请求，或进入丢队列，可以通过控制添加令牌的速率，来控制整体速度。Guava 中的 RateLimiter 是令牌桶的实现。
	* Nginx 限流：通过 `limit_req` 等模块限制并发连接数。

### 应用层容灾

* [《防雪崩利器：熔断器 Hystrix 的原理与使用》](https://segmentfault.com/a/1190000005988895)
	* 雪崩效应原因：硬件故障、硬件故障、程序Bug、重试加大流量、用户大量请求。 
	* 雪崩的对策：限流、改进缓存模式(缓存预加载、同步调用改异步)、自动扩容、降级。
	* Hystrix设计原则：
		* 资源隔离：Hystrix通过将每个依赖服务分配独立的线程池进行资源隔离, 从而避免服务雪崩。
		* 熔断开关：服务的健康状况 = 请求失败数 / 请求总数，通过阈值设定和滑动窗口控制开关。
		* 命令模式：通过继承 HystrixCommand 来包装服务调用逻辑。 

* [《缓存穿透，缓存击穿，缓存雪崩解决方案分析》](https://blog.csdn.net/zeb_perfect/article/details/54135506)
* [《缓存击穿、失效以及热点key问题》](https://blog.csdn.net/zeb_perfect/article/details/54135506) 
	* 主要策略：失效瞬间：单机使用锁；使用分布式锁；不过期；
	* 热点数据：热点数据单独存储；使用本地缓存；分成多个子key；

###跨机房容灾

* [《“异地多活”多机房部署经验谈》](http://dc.idcquan.com/ywgl/71559.shtml)
	* 通过自研中间件进行数据同步。 

* [《异地多活（异地双活）实践经验》](https://blog.csdn.net/jeffreynicole/article/details/48135093)
	* 注意延迟问题，多次跨机房调用会将延时放大数倍。
	* 建房间专线很大概率会出现问题，做好运维和程序层面的容错。
	* 不能依赖于程序端数据双写，要有自动同步方案。 
	* 数据永不在高延迟和较差网络质量下，考虑同步质量问题。
	* 核心业务和次要业务分而治之，甚至只考虑核心业务。
	* 异地多活监控部署、测试也要跟上。
	* 业务允许的情况下考虑用户分区，尤其是游戏、邮箱业务。
	* 控制跨机房消息体大小，越小越好。
	* 考虑使用docker容器虚拟化技术，提高动态调度能力。

* [容灾技术及建设经验介绍](https://blog.csdn.net/yoara/article/details/38013751)
	*  ​

### 容灾演练流程

* [《依赖治理、灰度发布、故障演练，阿里电商故障演练系统的设计与实战经验》](https://mp.weixin.qq.com/s?__biz=MjM5MDE0Mjc4MA==&mid=2650996320&idx=1&sn=0ed3be190bbee4a9277886ef88cbb2e5)
	* 常见故障画像
	* 案例：预案有效性、预案有效性、故障复现、架构容灾测试、参数调优、参数调优、故障突袭、联合演练。

### 平滑启动

* 平滑重启应用思路
1.端流量（如vip层）、2. flush 数据(如果有)、3, 重启应用

* [《JVM安全退出（如何优雅的关闭java服务）》](https://blog.csdn.net/u011001084/article/details/73480432)
推荐推出方式：System.exit，Kill SIGTERM；不推荐 kill-9；用 Runtime.addShutdownHook 注册钩子。
* [《常见Java应用如何优雅关闭》](http://ju.outofmemory.cn/entry/337235)
Java、Srping、Dubbo 优雅关闭方式。

## 数据库扩展

### 读写分离模式

* [《Mysql主从方案的实现》](https://www.cnblogs.com/houdj/p/6563771.html)
* [《搭建MySQL主从复制经典架构》](https://www.cnblogs.com/edisonchou/p/4133148.html)
* [《Haproxy+多台MySQL从服务器(Slave) 实现负载均衡》](https://blog.csdn.net/nimasike/article/details/48048341)

* [《DRBD+Heartbeat+Mysql高可用读写分离架构》](https://www.cnblogs.com/zhangsubai/p/6801764.html)
	* DRDB 进行磁盘复制，避免单点问题。

* [《MySQL Cluster 方式》](https://coderxing.gitbooks.io/architecture-evolution/di-san-pian-ff1a-bu-luo/62-ke-kuo-zhan-de-shu-ju-ku-jia-gou/621-gao-ke-yong-mysql-de-ji-zhong-fang-an/6214-mysql-cluster-fang-an.html)

### 分片模式
* [《分库分表需要考虑的问题及方案》](https://www.jianshu.com/p/32b3e91aa22c)
	* 中间件： 轻量级：sharding-jdbc、TSharding；重量级：Atlas、MyCAT、Vitess等。
	* 问题：事务、Join、迁移、扩容、ID、分页等。
	* 事务补偿：对数据进行对帐检查;基于日志进行比对;定期同标准数据来源进行同步等。
	* 分库策略：数值范围；取模；日期等。
	* 分库数量：通常 MySQL 单库 5千万条、Oracle 单库一亿条需要分库。 

* [《MySql分表和表分区详解》](https://www.2cto.com/database/201503/380348.html)
	* 分区：是MySQL内部机制，对客户端透明，数据存储在不同文件中，表面上看是同一个表。
	* 分表：物理上创建不同的表、客户端需要管理分表路由。

## 服务治理
###  服务注册与发现

* [《永不失联！如何实现微服务架构中的服务发现？》](https://blog.csdn.net/jiaolongdy/article/details/51188798)
  * 客户端服务发现模式：客户端直接查询注册表，同时自己负责负载均衡。Eureka 采用这种方式。
  * 服务器端服务发现模式：客户端通过负载均衡查询服务实例。
* [《SpringCloud服务注册中心比较:Consul vs Zookeeper vs Etcd vs Eureka》](https://blog.csdn.net/u010963948/article/details/71730165)
  * CAP支持：Consul（CA）、zookeeper（cp）、etcd（cp） 、euerka（ap）
  * 作者认为目前 Consul 对 Spring cloud 的支持比较好。

* [《基于Zookeeper的服务注册与发现》](http://mobile.51cto.com/news-502394.htm)
	* 优点：API简单、Pinterest，Airbnb 在用、多语言、通过watcher机制来实现配置PUSH，能快速响应配置变化。 

### 服务路由控制
* [《分布式服务框架学习笔记4 服务路由》](https://blog.csdn.net/xundh/article/details/59492750)
	* 原则：透明化路由
	* 负载均衡策略：随机、轮询、服务调用延迟、一致性哈希、粘滞连接
	* 本地路由有限策略：injvm(优先调用jvm内部的服务)，innative(优先使用相同物理机的服务),原则上找距离最近的服务。
	* 配置方式：统一注册表；本地配置；动态下发。

## 分布式一致

### CAP 与 BASE 理论

* [《从分布式一致性谈到CAP理论、BASE理论》](http://www.cnblogs.com/szlbm/p/5588543.html)
	* 一致性分类：强一致(立即一致)；弱一致(可在单位时间内实现一致，比如秒级)；最终一致(弱一致的一种，一定时间内最终一致)
	* CAP：一致性、可用性、分区容错性(网络故障引起)
	* BASE：Basically Available（基本可用）、Soft state（软状态）和Eventually consistent（最终一致性）
	* BASE理论的核心思想是：即使无法做到强一致性，但每个应用都可以根据自身业务特点，采用适当的方式来使系统达到最终一致性。

### 分布式锁

* [《分布式锁的几种实现方式》](http://www.hollischuang.com/archives/1716)
	* 基于数据库的分布式锁：优点：操作简单、容易理解。缺点：存在单点问题、数据库性能够开销较大、不可重入；
	* 基于缓存的分布式锁：优点：非阻塞、性能好。缺点：操作不好容易造成锁无法释放的情况。
	* Zookeeper 分布式锁：通过有序临时节点实现锁机制，自己对应的节点需要最小，则被认为是获得了锁。优点：集群可以透明解决单点问题，避免锁不被释放问题，同时锁可以重入。缺点：性能不如缓存方式，吞吐量会随着zk集群规模变大而下降。
* [《基于Zookeeper的分布式锁》](https://www.tuicool.com/articles/VZJr6fY)
	* 清楚的原理描述 + Java 代码示例。 

### 分布式一致性算法

####PAXOS
* [《分布式系列文章——Paxos算法原理与推导》](https://www.cnblogs.com/linbingdong/p/6253479.html)
* [《Paxos-->Fast Paxos-->Zookeeper分析》](https://blog.csdn.net/u010039929/article/details/70171672)
* [《【分布式】Zookeeper与Paxos》](https://www.cnblogs.com/leesf456/p/6012777.html)

#### Zab
* [《Zab：Zookeeper 中的分布式一致性协议介绍》](https://www.jianshu.com/p/fb527a64deee)

#### Raft
* [《Raft 为什么是更易理解的分布式一致性算法》](http://www.cnblogs.com/mindwind/p/5231986.html)

#### Gossip
* [《Gossip算法》](http://blog.51cto.com/tianya23/530743)

#### 两阶段提交、多阶段提交

* [《关于分布式事务、两阶段提交协议、三阶提交协议》](http://blog.jobbole.com/95632/)

### 幂等

* [《分布式系统---幂等性设计》](https://www.cnblogs.com/wxgblogs/p/6639272.html)
	* 幂等特性的作用：该资源具备幂等性，请求方无需担心重复调用会产生错误。
	* 常见保证幂等的手段：MVCC（类似于乐观锁）、去重表(唯一索引)、悲观锁、一次性token、序列号方式。 

### 分布式一致方案
* [《分布式系统事务一致性解决方案》](http://www.infoq.com/cn/articles/solution-of-distributed-system-transaction-consistency)
* [《保证分布式系统数据一致性的6种方案》](https://weibo.com/ttarticle/p/show?id=2309403965965003062676)

### 分布式 Leader 节点选举
* [《利用zookeeper实现分布式leader节点选举》](https://blog.csdn.net/johnson_moon/article/details/78809995)

### TCC(Try/Confirm/Cancel) 柔性事务
* [《传统事务与柔性事务》](https://www.jianshu.com/p/ab1a1c6b08a1)
	* 基于BASE理论：基本可用、柔性状态、最终一致。
	* 解决方案：记录日志+补偿（正向补充或者回滚）、消息重试(要求程序要幂等)；“无锁设计”、采用乐观锁机制。

## 分布式文件系统

* [说说分布式文件存储系统-基本架构](https://zhuanlan.zhihu.com/p/27666295) ？
* [《各种分布式文件系统的比较》](https://blog.csdn.net/gatieme/article/details/44982961) ？
  * HDFS：大批量数据读写，用于高吞吐量的场景，不适合小文件。
  * FastDFS：轻量级、适合小文件。

## 唯一ID 生成

### 全局唯一ID
* [《高并发分布式系统中生成全局唯一Id汇总》](https://www.cnblogs.com/baiwa/p/5318432.html)
	* Twitter 方案（Snowflake 算法）：41位时间戳+10位机器标识（比如IP，服务器名称等）+12位序列号(本地计数器)
	* Flicker 方案：MySQL自增ID + "REPLACE INTO XXX:SELECT LAST_INSERT_ID();" 
	* UUID：缺点，无序，字符串过长，占用空间，影响检索性能。
	* MongoDB 方案：利用 ObjectId。缺点：不能自增。

* [《TDDL 在分布式下的SEQUENCE原理》](https://blog.csdn.net/hdu09075340/article/details/79103851)
	* 在数据库中创建 sequence 表，用于记录，当前已被占用的id最大值。
	* 每台客户端主机取一个id区间（比如 1000~2000）缓存在本地，并更新 sequence 表中的id最大值记录。
	* 客户端主机之间取不同的id区间，用完再取，使用乐观锁机制控制并发。

## 一致性Hash算法

* [《一致性哈希算法》](https://coderxing.gitbooks.io/architecture-evolution/di-san-pian-ff1a-bu-luo/631-yi-zhi-xing-ha-xi.html)

# 设计思想 & 开发模式

## DDD(Domain-driven Design - 领域驱动设计)

* [《浅谈我对DDD领域驱动设计的理解》](https://www.cnblogs.com/netfocus/p/5548025.html)
  * 概念：DDD 主要对传统软件开发流程(分析-设计-编码)中各阶段的割裂问题而提出，避免由于一开始分析不明或在软件开发过程中的信息流转不一致而造成软件无法交付（和需求方设想不一致）的问题。DDD 强调一切以领域（Domain）为中心，强调领域专家（Domain Expert）的作用，强调先定义好领域模型之后在进行开发，并且领域模型可以指导开发（所谓的驱动）。
  * 过程：理解领域、拆分领域、细化领域，模型的准确性取决于模型的理解深度。
  * 设计：DDD 中提出了建模工具，比如聚合、实体、值对象、工厂、仓储、领域服务、领域事件来帮助领域建模。
  
* [《领域驱动设计的基础知识总结》](https://www.cnblogs.com/butterfly100/p/7827870.html)
  * 领域（Doamin）本质上就是问题域，比如一个电商系统，一个论坛系统等。
  * 界限上下文（Bounded Context）：阐述子域之间的关系，可以简单理解成一个子系统或组件模块。
  * 领域模型（Domain Model）：DDD的核心是建立（用通用描述语言、工具—领域通用语言）正确的领域模型；反应业务需求的本质，包括实体和过程；其贯穿软件分析、设计、开发 的整个过程；常用表达领域模型的方式：图、代码或文字；
  * 领域通用语言：领域专家、开发设计人员都能立即的语言或工具。
  * 经典分层架构：用户界面/展示层、应用层、领域层、基础设施层，是四层架构模式。
  * 使用的模式：
    * 关联尽量少，尽量单项，尽量降低整体复杂度。
    * 实体（Entity）：领域中的唯一标示，一个实体的属性尽量少，少则清晰。
    * 值对象（Value Object）：没有唯一标识，且属性值不可变，小二简单的对象，比如Date。
    * 领域服务（Domain Service）： 协调多个领域对象，只有方法没有状态(不存数据)；可以分为应用层服务，领域层服务、基础层服务。
    * 聚合及聚合根（Aggregate，Aggregate Root）：聚合定义了一组具有内聚关系的相关对象的集合；聚合根是对聚合引用的唯一元素；当修改一个聚合时，必须在事务级别；大部分领域模型中，有70%的聚合通常只有一个实体，30%只有2~3个实体；如果一个聚合只有一个实体，那么这个实体就是聚合根；如果有多个实体，那么我们可以思考聚合内哪个对象有独立存在的意义并且可以和外部直接进行交互；
    * 工厂（Factory）：类似于设计模式中的工厂模式。
    * 仓储（Repository）：持久化到DB，管理对象，且只对聚合设计仓储。

* [《领域驱动设计(DDD)实现之路》](http://www.cnblogs.com/Leo_wl/p/3866629.html)
	* 聚合：比如一辆汽车（Car）包含了引擎（Engine）、车轮（Wheel）和油箱（Tank）等组件，缺一不可。

* [《领域驱动设计系列（2）浅析VO、DTO、DO、PO的概念、区别和用处》](http://www.hollischuang.com/archives/553)


### 命令查询职责分离(CQRS)

CQRS — Command Query Responsibility Seperation

* [《领域驱动设计系列 (六)：CQRS》](https://www.cnblogs.com/cnblogsfans/p/4551990.html)
	* 核心思想：读写分离（查询和更新在不同的方法中），不同的流程只是不同的设计方式，CQ代码分离，分布式环境中会有明显体现（有冗余数据的情况下），目的是为了高性能。

* [《DDD CQRS架构和传统架构的优缺点比较》](http://www.techweb.com.cn/network/system/2017-07-07/2553563.shtml)
	* 最终一致的设计理念；依赖于高可用消息中间件。
	
* [《CQRS架构简介》](http://www.cnblogs.com/netfocus/p/4055346.html)
	* 一个实现 CQRS 的抽象案例。

* [《深度长文：我对CQRS/EventSourcing架构的思考》](http://www.uml.org.cn/zjjs/201609221.asp)
	* CQRS 模式分析 + 12306 抢票案例

### 贫血，充血模型

* [《贫血，充血模型的解释以及一些经验》](https://kb.cnblogs.com/page/520743/)
	* 失血模型：老子和儿子分别定义，相互不知道，二者实体定义中完全没有业务逻辑，通过外部Service进行关联。
	* 贫血模型：老子知道儿子，儿子也知道老子；部分业务逻辑放到实体中；优点：各层单项依赖，结构清楚，易于维护；缺点：不符合OO思想，相比于充血模式，Service层较为厚重；
	* 充血模型：和贫血模型类似，区别在于如何划分业务逻辑。优点：Service层比较薄，只充当Facade的角色，不和DAO打交道、复合OO思想；缺点：非单项依赖，DO和DAO之间双向依赖、和Service层的逻辑划分容易造成混乱。
	* 肿胀模式：是一种极端情况，取消Service层、全部业务逻辑放在DO中；优点：符合OO思想、简化了分层；缺点：暴露信息过多、很多非DO逻辑也会强行并入DO。这种模式应该避免。
	* 作者主张使用贫血模式。
	
## Actor 模式

TODO

## 响应式编程

TODO


# 项目管理

## 架构评审
* [《架构设计之如何评审架构设计说明书》](http://developer.51cto.com/art/201506/478486.htm)
* [《人人都是架构师：非功能性需求》](https://blog.csdn.net/wireless_com/article/details/45935591)

## 重构

TODO


## 代码规范


## RUP
* [《运用RUP 4+1视图方法进行软件架构设计》](https://blog.csdn.net/apanious/article/details/51011946)

## 看板管理
* [《说说看板在项目中的应用》](https://blog.csdn.net/tkchen/article/details/51637643)

## SCRUM

* [《敏捷项目管理流程-Scrum框架最全总结！》](https://blog.csdn.net/inny100_100/article/details/54633757)

## 极限编程

TODO

## 敏捷开发

TODO

## 结对编程

TODO

# 通用业务术语

TODO

#技术趋势

TODO

#架构师素质

* [《架构师画像》](http://hellojava.info/?p=430)
	* 业务理解和抽象能力
	* NB的代码能力
	* 全面：1. 在面对业务问题上，架构师脑海里是否会浮现出多种技术方案；2. 在做系统设计时是否考虑到了足够多的方方面面；3. 在做系统设计时是否考虑到了足够多的方方面面； 
	* 全局：是否考虑到了对上下游的系统的影响。
	* 权衡：权衡投入产出比；优先级和节奏控制；

* [《关于架构优化和设计，架构师必须知道的事情》](http://www.infoq.com/cn/articles/architecture-optimization-and-design-the-architect-must-know)
	* 要去考虑的细节：模块化、轻耦合、无共享架构；减少各个组件之前的依懒、注意服务之间依懒所有造成的链式失败及影响等。
	* 基础设施、配置、测试、开发、运维综合考虑。
	* 考虑人、团队、和组织的影响。 

* [《如何才能真正的提高自己，成为一名出色的架构师？》](https://www.zhihu.com/question/19841397) 

* [《架构师的必备素质和成长途径》](https://blog.csdn.net/sanbingyutuoniao123/article/details/54144129)
	* 素质：业务理解、技术广度、技术深度、丰富经验、沟通能力、动手能力、美学素养。
	* 成长路径：2年积累知识、4年积累技能和祖内影响力、7年积累部门内影响力、7年以上积累跨部门影响力。 

* [《架构设计师—你在哪层楼？》](http://blog.51cto.com/frankfan/1248401)
	* 第一层的架构师看到的只是产品本身
	* 第二层的架构师不仅看到自己的产品，还看到了整体的方案
	* 第三层的架构师看到的是商业价值 

#团队管理

TODO

# 资讯

## 行业资讯

* [36kr](http://36kr.com/)

## 公众号列表

TODO

## 博客

### 团队博客
* [阿里中间件博客](http://jm.taobao.org/)
* [美团点评技术团队博客](https://tech.meituan.com)

### 个人博客

* [阮一峰的网络日志](http://www.ruanyifeng.com/)
* [酷壳 - COOLSHELL-陈皓](https://coolshell.cn/)
* [hellojava-阿里毕玄](http://hellojava.info/)

## 综合门户、社区

**国内：**

* [CSDN](http://csdn.net)
	 老牌技术社区、不必解释。
* [Techweb](http://www.techweb.com.cn/)
	* 新闻类内容居多。	
* [51cto.com](http://www.51cto.com/)
* [ITeye](http://www.iteye.com/)
	* 偏 Java 方向 
* [博客园](https://www.cnblogs.com)
* [ChinaUnix](http://www.tom.net/)
	* 偏 Linux 方向 
* [开源中国社区](https://www.oschina.net/)
* [深度开源](http://www.open-open.com/)
* [伯乐在线](http://www.jobbole.com/)
	* 涵盖 IT职场、Web前端、后端、移动端、数据库等方面内容，偏技术端。

* [ITPUB](http://www.itpub.net/)
* [腾讯云— 云+社区](https://cloud.tencent.com/developer/column)
* [阿里云— 云栖社区](https://yq.aliyun.com/)
* [IBM DeveloperWorks](https://www.ibm.com/developerworks/cn/)
* [开发者头条](https://toutiao.io/)
* [LinkedKeeper](http://www.linkedkeeper.com)

**国外：**

* [DZone](https://dzone.com)
* [Reddit](https://www.reddit.com)

## 问答、讨论类社区

* [segmentfault](https://segmentfault.com)
	* 问答+专栏 
* [知乎](https://www.zhihu.com/)
* [stackoverflow](https://stackoverflow.com/)

## 专项网站

* 测试:
	* [领测国际](http://www.ltesting.net/) 
	* [测试窝](https://www.testwo.com/)
	* [TesterHome](https://testerhome.com)

* 运维:
  * [运维派](http://www.yunweipai.com/) 

* Java:
	* [ImportNew](http://www.importnew.com/)
		* 专注于 Java 技术分享 	
* 安全
	* [红黑联盟](https://www.2cto.com/) 

* 大数据
	* [中国大数据](http://www.thebigdata.cn/) 

* 其他专题网站：
	* [DockerInfo](http://www.dockerinfo.net/)
		* 专注于 Docker 应用及咨询、教程的网站。
	* [Linux公社](https://www.linuxidc.com/)
		* Linux 主题社区

## 其他类

* [程序员技能图谱](https://github.com/TeamStuQ/skill-map)

## 推荐参考书

* [gitbook.com](http://gitbook.com)
* [gitbook.cn](http://gitbook.cn/)
	* 付费电子书。 

### 在线电子书

* [《深入理解Spring Cloud与微服务构建》](https://github.com/forezp/SpringCloudLearning)

### 纸质书

* 《软件架构师的12项修炼：技术技能篇》[京东](http://item.jd.com/11740744.html?cpdad=1DLSUE)
* 《架构之美》
* 《分布式服务架构》

# 技术资源

## 开源资源

* [github](https://github.com)

## 手册

* [W3Cschool](http://w3cschool.cn) 
* [Runoob.com](http://www.runoob.com/)
	* HTML 、 CSS、XML、Java、Python、PHP、设计模式等入门手册。

## 在线课堂

* [学徒无忧](http://www.xuetuwuyou.com/)
* [极客时间](https://time.geekbang.org/)
* [segmentfault](https://segmentfault.com/lives)
* [斯达克学院](https://new.stuq.org/course/explore)
* [牛客网](http://nowcoder.com)

## 会议

* [QCon](http://www.infoq.com/cn/qcon/)
* [ArchSummit](https://archsummit.com)

## 工具

* [极客搜索](https://s.geekbang.org/)
	* 技术文章搜索引擎。

## 文件服务
* 七牛
* 又拍云

## 综合云服务商
* 阿里云
* 腾讯云
* 百度云
* 新浪云
* 金山云