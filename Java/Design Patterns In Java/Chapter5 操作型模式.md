### 21.模板方法模式
在方法中实现算法, 推迟对算法步骤的定义使得子类能够重新实现

在一个方法中实现一个算法, 并推迟定义算法的某些步骤, 从而让其他类重新定义他们

比如排序算法 和Comparable接口, 只要修改Comparable接口, 就可以对排序算法进行重用

### 22.状态模式
将操作分散, 使得每个类都能够表示不同的状态

将表示对象状态的逻辑分散到代表状态的不同类中

例子:abstract class DoorState

class DoorOpened extends DoorState


##### 认识状态模式
　　●　　状态和行为

　　所谓对象的状态，通常指的就是对象实例的属性的值；而行为指的就是对象的功能，再具体点说，行为大多可以对应到方法上。

　　状态模式的功能就是分离状态的行为，通过维护状态的变化，来调用不同状态对应的不同功能。也就是说，状态和行为是相关联的，它们的关系可以描述为：状态决定行为。



　　●　　行为的平行性

　　注意平行线而不是平等性。所谓平行性指的是各个状态的行为所处的层次是一样的，相互独立的、没有关联的，是根据不同的状态来决定到底走平行线的哪一条。行为是不同的，当然对应的实现也是不同的，相互之间是不可替换的。



　　● 　　环境和状态处理对象

　　在状态模式中，环境(Context)是持有状态的对象，但是环境(Context)自身并不处理跟状态相关的行为，而是把处理状态的功能委托给了状态对应的状态处理类来处理。
  
  ### 23.策略模式
  封装操作, 使得实现是可以互相替换的

策略模式是将可互换的方法封装在各自独立的类中, 并且让每个方法都实现一个公共的操作

例子: 广告推荐模型: 抽象类Advisor, 方法recommend, 
具体类:groupAdvisor, itemAdvisor, 这两个类实现了共同的操作接口

例子2:交通工具(抽象类)
具体类:公交车, 地铁, 自行车 都实现了到达目的地的接口


### 24.命令模式
用对象来封装方法调用

命令模式是将请求封装在对象内部


### 25.解释器模式
将操作分散, 使得每个实现能够运用到不同类型的集合中

解释器模式让你根据实现定义好的一系列组合规则, 组合可执行对象

向计算机输入一个句子或文件，它就能够按照预先定义的文法规则来对句子或文件进行解释，从而实现相应的功能。例如提供一个简单的加法/减法解释器，只要输入一个加法/减法表达式，它就能够计算出表达式结果

在以下情况下可以考虑使用解释器模式： 
(1) 可以将一个需要解释执行的语言中的句子表示为一个抽象语法树。 
(2) 一些重复出现的问题可以用一种简单的语言来进行表达。 
(3) 一个语言的文法较为简单。 
(4) 执行效率不是关键问题。


