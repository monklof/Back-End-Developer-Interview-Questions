后端开发者面试题
================

## 说明

这篇文章翻译自一位外国友人的关于面试后端程序员的文章，我比较喜爱这篇文章，认为它不仅对于面试者，对于面试官来说也是个不错的参考。于是迫不及待的翻译了一下，给各位看官做个参考。

原文参见: https://github.com/arialdomartini/Back-End-Developer-Interview-Questions

以下是原文翻译。

后端开发者面试题
================

在面试的时候，我并不特别喜欢问一些技术性的问题。我更喜欢的方式是这样的: 和面试者坐在一起，看一些实际的代码，解决一些实际的问题。并且用一整天的时间，让团队所有成员轮流和面试者进行结对编程。虽然如此，但是一些技术问题仍然可以用来很好地启动一段有深度的谈话，能够让面试者和面试官相互都有更加深入的了解。

这个仓库包含了可以用来考核面试者的一系列后端面试题。绝不是说，面试官必须用每个面试题来考核面试者（这样可能要耗费好几个小时）。根据你期望面试者拥有的技能，从这个列表中有选择的挑一些题目，可以帮助你在特定技能上考核面试者。

应当承认的是，这个项目的灵感来自于[@darcyclarke](https://github.com/darcyclarke)的文章[Front-end Job Interview Questions](https://github.com/darcyclarke/Front-end-Developer-Interview-Questions)

**注意:** 请记住，这些面试题中有许多问题是开放式的，能引导讨论一些有趣的问题。相比那些有直接答案的问题来说，这种问题能够让你对面试者的能力有更多的了解。再一次强调，我认为仅仅是问问题是不够的。要通过与面试者较长时间的结对编程来完成面试: 这是你们相互了解对方风格和手段、让面试者了解未来工作的最佳手段之一。

## <a name='toc'>目录</a>

  1. [通用问题](#general)
  1. [开放式问题](#open)
  1. [设计模式相关问题](#patterns)
  1. [代码设计相关问题](#design)
  1. [语言相关问题](#languages)
  1. [Web相关问题](#web)
  1. [数据库相关问题](#databases)
  1. [非关系型数据库相关问题](#nosql)
  1. [代码版本管理相关问题](#codeversioning)
  1. [并发问题](#concurrency)
  1. [分布式系统相关问题](#distributed)
  1. [软件生命周期和团队管理相关问题](#management)
  1. [逻辑和算法相关问题](#algorithms)
  1. [软件架构相关问题](#architecture)
  1. [面向服务架构(SOA)和微服务(Microservice)相关问题](#soa)
  1. [安全相关问题](#security)
  1. [比尔盖茨式问题](#billgates)
  1. [代码示例问题](#snippets)

####[[↑]](#toc) <a name='general'>通用问题:</a>

* Remove the concept of "null" from your preferred language.
* 为什么函数式编程重要？什么时候可以使用函数式语言？
* 设计(design)、架构(architecture)、功能(functionality)和美学(aesthetic)之间有什么区别？讨论一下。
* 微软、谷歌、欧朋(opera)和火狐这类公司是如何从他们的浏览器中获利的？
* 为什么打开TCP套接字有很大的开销？
* 封装的重要性体现在哪儿？
* 什么是实时系统？它与普通系统有什么区别？
* What's the relationship between real-time languages and heap memory allocation?
* 不变性(Immutability)是指在实践中，(变量的)值只能在创建的时候被设置一次，之后就不能被改变。为什么不变性能帮助写更加安全的代码？
* 可变(mutable)值和不可变(unmutable)值有哪些利弊？
* 什么是O/R阻抗失衡(Object-Relational impedence mismatch)？
* 如果你需要使用缓存，你使用哪些原则来确定缓存的大小？
* TCP和HTTP有什么区别？
* 在客户端渲染(client-side rendering)和服务端渲染(server-side rendering)之间，你如何权衡？
* 你如何在一个不可靠的协议之上构建一个可靠的通信协议？

####[[↑]](#toc) <a name='open'>开放式问题:</a>

* 为什么人们会抵制变化？
* 如何向你的祖母解释什么是线程？
* 作为一个软件工程师，你想要既有创新力又有可预测性。采用什么策略才能使这两个目标可以共存呢？
* 什么是好的代码？
* 解释什么是流(Streaming)和你能如何实现它？
* 假设你的公司给你一周的时间，让你提高你和同事的生活: 你将如何使用这一周？
* 本周你学了什么？
* 所有的设计中都会有美学元素(aesthetic element)的存在。问题是，你认为美学元素是你的朋友还是敌人？
* 列出最近你读过的5本书。
* How would you introduce Continue Delivery in a multi million waterfall shop?
* 我们来谈谈"*重复造轮子*","*非我发明症*", "*吃自己做出来的狗粮*"的这些做法吧。(Reinventing the wheel, Not Invented Here Syndrome, Eating Your Own Food)
* 在你当前的工作流中，什么事情是你下一步需要自动化的？
* 为什么写软件是困难的？是什么使软件的维护变得困难？
* 你更喜欢在全新项目（Green Field Project）上工作还是在扩建项目(Brown Field Project)上工作？为什么？
* [当你在浏览器地址栏输入google.com回车之后都发生了什么?](https://github.com/alex/what-happens-when)
* What does your computer do when you wait?
* 如何向一个5岁的孩子解释什么是Unicode/数据库事务？
* 如何维护单体架构(monolithic architecture)？
* 你如何理解"专家"？
* 软件开发是一门艺术、一门技艺还是一种工程？你的观点是什么？
* "喜欢这个的人也喜欢..."，你如何在一个电子商务商店上实现这种功能？
* 为什么在创新上，企业会比创业公司做得慢？

####[[↑]](#toc) <a name='patterns'>设计模式相关问题:</a>

* 请用一个例子表明，全局对象是邪恶的存在？
* 假设你工作的系统不支持事务性，你会如何从头开始实现它？
* 什么是好莱坞原则（Hollywood Principles）？
* 关于迪米特法则(最少知识原则): 写一段代码违反它, 然后修复它。

（注: 迪米特法则：the Law of Demeter, 最少知识原则： the Principle of Least Knowledge）
* Active-Record模式有什么限制和缺陷？
* Data-Mapper模式和Active-Record模式有什么区别？
* 空对象模式(Null Object Pattern)的目的是什么？
* 为什么组合(Composition)比继承(Inheritance)更加有好？
* 什么是反腐败层(Anti-corruption Layer)?
* 你可以写一个线程安全的单例(Singleton)类吗？
* Could you implement Objects in terms of Higher Order Functions, and vice-versa?
* 数据抽象(Data Abstraction)能力是指能改变实现而不影响客户端的这种能力。请构造一个一个例子，违反这个特性，并且尝试修复它。
* 你是如何处理依赖关系地狱(Dependency Hell)的？
* 为什么goto语句是恶魔班的存在？

####[[↑]](#toc) <a name='design'>代码设计相关问题:</a>

* What is the tests influence on design?
* 内聚和耦合的区别是什么？
* 重构在哪些场景下有用？
* 代码中的注释有用吗？
* 设计和架构有什么区别？
* 为什么在测试驱动开发(TDD)中弦写测试，再写代码？
* C++支持多继承，Java允许类实现多个接口。这些特性对正交性有什么影响？使用多继承和使用多接口有区别吗？[这个问题来自Andrew .Hunt 和 David Thomas写的《程序员修炼之道》]

####[[↑]](#toc) <a name='languages'>语言相关问题:</a>

* 告诉我你钟爱的语言的三个最坏的缺陷
* 为什么现在函数式编程这么越来越受关注？
* 闭包是什么？它有什么用途？闭包和类有什么共同点？
* 泛型有什么用途？
* 什么是高阶函数？有什么用途？用你的首选语言写个例子出来。
* Write a loop, then transform it into a recursive function, avoiding mutability. Discuss. 
* 一个语言将函数视为第一公民，这是什么意思？
* 用一个例子说明匿名函数其实是有用的。
* 什么是动态方法调度(Dynamic Method Dispatch)？
* 名字空间(Namespace)有什么用？有什么可以替代它的吗？
* 谈谈Java和C#之间的互操作性(Interoperability) (任选其他两门语言都行)
* 为什么很多软件工程师不喜欢Java？
* 你认为好的语言好在哪里？差的语言差在哪里？
* 写两个函数，一个是"引用透明的(Referentially Transparent)"，另一个是"引用不透明的(Referentially Opaque)"。讨论之。
* 什么是栈？什么是堆？
* 为什么一个语言中，"函数是第一公民"是很重要的？
* How is Pattern Matching different than Switch clauses?
* 为什么有些语言设计上没有异常机制？这有什么优劣？
* 如果`Cat`是一个`Animal`, 那么`TaskCare<Cat>`是一个`TakeCare<Animal>`吗？

####[[↑]](#toc) <a name='web'>web相关问题:</a>

* 为什么"第一方cookie(first-party cookie)"和"第三方cookie(third-party cookie)"被如此不同的对待？

####[[↑]](#toc) <a name='databases'>数据库相关问题:</a>

* 如果要你将一个项目从MySQL迁移至PostgreSQL中，你会如何进行这个迁移？
* 为什么```SELECT * FROM table WHERE field = null```不能匹配空的字段？
* 什么是ACID(原子性，一致性，隔离性，持久性)
* 你是如何进行数据库模式(Database schema)迁移的？
* 延迟加载(lazy loading)是如何实现的？什么场景下有用？他有什么缺陷？
* 什么是N+1问题？
* 如何找出应用中开销最大的查询？

####[[↑]](#toc) <a name='nosql'>非关系型数据库相关问题:</a>

* 什么是最终一致性(Eventual Consistency)？
* 关于CAP理论，举一些CP、AP、CA系统的例子。
* NoSQL是如何解决可伸缩性的挑战的？

####[[↑]](#toc) <a name='codeversioning'>代码版本管理相关问题:</a>

* 为什么在Mercurial或者git中(管理)分支比SVN容易？
* 分散式版本控制系统（比如git），相比集中式版本控制系统（如svn）有哪些优势和劣势？

(注:
* 分散式版本控制系统: Centralized Version Control Systems
* 集中式版本控制系统: Distributed Version Control Systems)

* 能描述一下什么是GitHubFlow和GitFlow工作流吗？
* 什么是rebase？
* 为什么合并操作(merge)在Mercurial和git中比在SVN和CVS中容易？

####[[↑]](#toc) <a name='concurrency'>并发问题:</a>

* 为什么我们需要并发呢？解释一下。
* 为什么测试多线程/并发代码这么困难？
* 什么是竞争条件（Race Condition）？用任何一个语言写一个例子。
* 什么是死锁？用代码解释一下。
* 什么是饿死？
* 什么是Wait-Free算法？

####[[↑]](#toc) <a name='distributed'>分布式系统相关问题:</a>

* 怎么测试一个分布式系统？
* 什么场景下你会在两个系统中采用异步通信机制？
* 远程过程调用的通用缺点是什么？
* 如果你为了可扩展性和鲁棒性而构建一个分布式的系统，在封闭安全的网络环境下和地理上的位置不同但是网络环境不是封闭和安全的，这两种情况下你会考虑什么不同的事情？
* 在Web应用中如何管理容错性？在桌面端呢？
* 在分布式系统中，如何处理故障？
* 让我们来谈谈网络分裂(network partitions)后有的几种恢复的手段吧。
* 你认为分布式计算中有哪些谬论？
* 你在什么时候会使用Request/Response模式，什么时候使用Publish/Subscribe模式？

####[[↑]](#toc) <a name='management'>软件生命周期和团队管理相关问题:</a>


####[[↑]](#toc) <a name='algorithms'>逻辑和算法相关问题:</a>

####[[↑]](#toc) <a name='architecture'>软件架构相关问题:</a>

####[[↑]](#toc) <a name='soa'>面向服务架构(SOA)和微服务(Microservice)相关问题:</a>

####[[↑]](#toc) <a name='security'>安全相关问题:</a>

####[[↑]](#toc) <a name='billgates'>比尔盖茨式问题:</a>

####[[↑]](#toc) <a name='snippets'>代码示例问题:</a>


