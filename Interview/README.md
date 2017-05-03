Hello Interview
===
## 测试相关
### 1. 自动化
---
1. **后台**
后台自动化主要涉及到shell,包括expect, 和python脚本, shell脚本没什么好说的, expect脚本主要用于远程登录其他环境获取文件,执行命令等. 而python脚本则多数作为爬虫使用在web页面上下载文件.

2. **smartAction**
smartAction是华为2012实验室开发的一个自动化工具, 搭配自动化框架TMSS使用. 首先, 使用Http Watch进行web录制, 将请求数据保存为一个xml文件, 然后使用自动解析工具, 保留客户端的请求信息并替换ip等变量, 最后我将xml中的其他需要替换的字段替换成变量, 变量通常使用xpath获取.

3. **smartGUI**
smartGUI是华为2012实验室开发的一个自动化工具, 类似于业界的QTP, 首先使用工具录制web页面, 并保存为一个map文件, 然后将部分字段替换为变量, 保存作为用例, 然后就可以执行了

### 2. 性能
***
我对性能测试接触得相对较少, 主要分两种, 1是使用自己编写的模拟桩作为业务网元连接到uniagent, 然后频繁调用模拟桩, 观察uniagent的资源消耗情况, 还有一种就是使用谷歌浏览器观察页面加载的速度. 没搞过web方面的性能测试. 不过我觉得自动化就是性能测试的基石, 会了自动化测试, 性能测试也不是难事.

### 3.安全性
对于SQL注入/XSS注入有一定的了解, 更了解的是sudo越权方面的, 因为我们的产品大多数为后台产品.

### other
 1. 先自我介绍一下吧！
    你好, 我叫赵仲禹, 毕业于武汉大学数学与统计学院信息与计算科学专业, 2014年进入中软国际任职软件测试工程师, 经过3年的工作经历, 对软件测试有了较多的了解, 熟悉软件测试的理论和流程, 熟悉shell和java/python语言, 对编程有一定的基础, 善于发现问题, 解决问题.个人性格开朗, 稳重, 具有高度的责任感, 适应力强, 能够不断地完善自我, 提高自身素质, 融入新环境.
软件测试工作方面的问题：
   2. 完成过软件测试的具体项目及知道它的职责吗？
      我前后经历了三个项目, 分别是华为的ATAE系统, I2000系统, 和DV系统.软件测试的职责在于制定测试计划,设计测试用例,提交测试报告,跟踪问题状态,推动问题解决.
   3. 平时工作除了软件测试，还有什么内容？
      维护测试环境, 输出经验文档, 支撑现网问题定位等.
   4. 软件测试遇到版本迭代，你如何处理？
   5. 如何编写测试用例，保证版本迭代？
      准备一份关键的门槛测试用例, 最好实现自动化, 并针对每个版本迭代中增删功能做一定修改, 当迭代中的包满足这份测试用例时, 基本可以认为这个包的基本功能是正常的.
   6. 软件测试经历中，你最有成就的案例，并详细介绍一下。
      软件测试的经历中遇到的问题大多都比较平淡, 如果非要说最有成就的那个案例,我想应该是我第一次接触到sudo越权的时候, 那时候我对shell脚本刚有初步的掌握, 在查看sudo配置的时候发现了存在越权的可能性, 比如直接拼接输入参数作为路径执行, 执行低权限的脚本, 以及直接使用eval命令等. 这一次的经历肯定了我对shell脚本的掌握, 让我的对这一块有了自信.
   7. 如有bug，如何和开发人员沟通？
      首先自己初步定位是否是BUG, 还是环境异常, 如果确定是问题并且能确定问题发生的原因, 则知会开发人员后直接提单, 如果无法确定是否是问题, 则保留环境, 知会开发人员定位问题.
   8. 软件测试用例的模型，如果发现迭代，如何优化版本？
      不好意思, 我在工作中没有接触过软件测试用例的模型是什么概念. 在我工作经历中, 我觉得迭代优化版本最重要的在于事后回顾,漏测分析.
   9. 流程有误觉得不好的地方，如果测试文档不全，你如何与相关人员沟通？
      通常来说我会选择直说, 要求相关人员补全文档, 提高相关的技术支撑.
   10. 遇到紧急上线，测试不能上线，如何和开发人员沟通?
       与开发沟通所发现的问题, 讨论其影响和严重性等, 尽量说服开发人员此问题的影响.
   11. 如果产品上线出现bug，研发人员不认为是bug，软件测试人员不认为是bug，如何处理？
       在华为, 客户认为的bug一定是bug, 我们能做的只是尽力说服客户, 让客户觉得这个不是bug. 要么说服, 要么改进.
   12. 你以往的工作中web测试的经验。
       我的以往工作项目中, 相对于web更关注在后台的运行, 对于web测试印象最深刻的还是对xss和sql注入攻击, 当然对于web测试中输入校验, 浏览器兼容性测试等测试也有一定了解, 印象中我们的产品web页面出现问题的地方主要在于浏览器兼容性, 前台做了合法性校验但是后台没有做导致可以绕过前台输入非法字符,错误信息未经处理直接抛出等.
   13. http使用经验，操作系统的使用和数据库的使用？
       对于数据库的使用, 我这边仅限于增删改查, 对于权限赋予等操作不熟, http的使用经验不知道知道是什么, 对于操作系统的使用, 还算比较熟.
### 3. 功能
***
等价类划分,边界值分析, 错误推测法, 因果图, 判定表,功能图

程序结构分析, 逻辑覆盖
逻辑覆盖有语句覆盖,判定条件覆盖, 路径覆盖

## 设计模式

工厂模式 -- 静态工厂模式
抽象工厂模式
建造者模式
单例模式
观察者模式

## 编程
### Python
1. Python的三种拷贝模式
* 直接传递引用
* 使用copy.copy浅拷贝, 这种情况下拷贝得到的对象如果包含子对象则子对象不会拷贝
* 使用copy.deepcopy深拷贝, 这种情况下拷贝得到的对象对包含的子对象也会进行拷贝

2. Python的socket


### java
1. java的垃圾管理机制
java使用被称作垃圾收集器的技术来监控java程序的运行, 当对象不再使用时就自动释放对象占用的内存. java使用软指针来跟踪对象的每个引用, 并用一个对象表映射为对象的引用.
垃圾收集器是自动运行的, 可以通过System.gc()来显式调用垃圾收集器, 但不能保证立即回收指定的对象.

2.堆和栈的区别
在java中, 使用new申请的对象都存放在堆内存中, 并将其指针变量存放到栈中, 其他对象则存放在栈中


### Linux
1. 软连接和硬链接的区别
创建硬链接时, 新的硬链接直接指向硬盘中的区块, 删除原先的文件, 硬链接不受影响.而创建软连接时, 软连接指向当前的文件名, 删除原先的文件,软连接就无法使用. 其实所有非软连接的文件都可以视为硬链接.

### 数据结构
链表/顺序表/队列/栈/二叉树/B树/B+树

## 网络
OSI七层结构从上到下依次是：
　　7 应用层 ;6 表示层 ;5 会话层 ;4 传输层 ;3 网络层 ;2 数据链路层 ;1 物理层
　　TCP/IP五层结构是
　　4 应用层;3 传输层; 2 网络互连层 1 主机到网络层


