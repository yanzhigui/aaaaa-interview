## JAVA

### 关键字

void byte int long char short float double String StringBuffer StringBuilder Array Collection Collections List ArrayList LinkedList Vector Set HashMap TreeMap LinkedHashMap ConcerrentHashMap Set TreeMap HashMap synchronized volatile transient implements extends public private protected this super static final const null run start thread enmu quicksort mergesort heapsort bubblesort selectsort insertsort stack queue list heap tree avlTree Btree B+Tree RTree throw throws try catch finally break continue instanceof

### java基础

#### 概念

- 面向对象的三大基本特征

    >三大特性是：封装,继承,多态  
    >
    >所谓封装，也就是把客观事物封装成抽象的类，并且类可以把自己的数据和方法只让可信的类或者对象操作，对不可信的进行信息隐藏。封装是面向对象的特征之一，是对象和类概念的主要特性。 简单的说，一个类就是一个封装了数据以及操作这些数据的代码的逻辑实体。在一个对象内部，某些代码或某些数据可以是私有的，不能被外界访问。通过这种方式，对象对内部数据提供了不同级别的保护，以防止程序中无关的部分意外的改变或错误的使用了对象的私有部分。
    >
    >
    >所谓继承是指可以让某个类型的对象获得另一个类型的对象的属性的方法。它支持按级分类的概念。继承是指这样一种能力：它可以使用现有类的所有功能，并在无需重新编写原来的类的情况下对这些功能进行扩展。 通过继承创建的新类称为“子类”或“派生类”，被继承的类称为“基类”、“父类”或“超类”。继承的过程，就是从一般到特殊的过程。要实现继承，可以通过“继承”（Inheritance）和“组合”（Composition）来实现。继承概念的实现方式有二类：实现继承与接口继承。实现继承是指直接使用基类的属性和方法而无需额外编码的能力；接口继承是指仅使用属性和方法的名称、但是子类必须提供实现的能力；
    >
    > 
    >
    >所谓多态就是指一个类实例的相同方法在不同情形有不同表现形式。多态机制使具有不同内部结构的对象可以共享相同的外部接口。这意味着，虽然针对不同对象的具体操作不同，但通过一个公共的类，它们（那些操作）可以通过相同的方式予以调用。
    >
    >
    >五大基本原则 
    >单一职责原则SRP(Single Responsibility Principle)
    是指一个类的功能要单一，不能包罗万象。如同一个人一样，分配的工作不能太多，否则一天到晚虽然忙忙碌碌的，但效率却高不起来。
    >
    >开放封闭原则OCP(Open－Close Principle) 
    一个模块在扩展性方面应该是开放的而在更改性方面应该是封闭的。比如：一个网络模块，原来只服务端功能，而现在要加入客户端功能，
    那么应当在不用修改服务端功能代码的前提下，就能够增加客户端功能的实现代码，这要求在设计之初，就应当将服务端和客户端分开，公共部分抽象出来。
    >
    >替换原则(the Liskov Substitution Principle LSP) 
    子类应当可以替换父类并出现在父类能够出现的任何地方。比如：公司搞年度晚会，所有员工可以参加抽奖，那么不管是老员工还是新员工，
    也不管是总部员工还是外派员工，都应当可以参加抽奖，否则这公司就不和谐了。
    >
    >依赖原则(the Dependency Inversion Principle DIP) 具体依赖抽象，上层依赖下层。假设B是较A低的模块，但B需要使用到A的功能，
    这个时候，B不应当直接使用A中的具体类： 而应当由B定义一抽象接口，并由A来实现这个抽象接口，B只使用这个抽象接口：这样就达到
    了依赖倒置的目的，B也解除了对A的依赖，反过来是A依赖于B定义的抽象接口。通过上层模块难以避免依赖下层模块，假如B也直接依赖A的实现，那么就可能造成循环依赖。一个常见的问题就是编译A模块时需要直接包含到B模块的cpp文件，而编译B时同样要直接包含到A的cpp文件。
    >
    >接口分离原则(the Interface Segregation Principle ISP) 
    模块间要通过抽象接口隔离开，而不是通过具体的类强耦合起来
    >    
- 面向过程、面向对象、基于对象和继承、派生、多态：http://www.i3geek.com/archives/580
- 编程思想，幻数：http://www.i3geek.com/archives/622

#### 集合类：

- JAVA高级——集合类 http://www.i3geek.com/archives/616  
- 详细阐述集合类   http://www.i3geek.com/archives/1233
- HashMap实现原理,源码阅读 http://www.i3geek.com/archives/1262
- HashMap中Key的约束
    >Map 描述了（key： value）成对放置的集合，key不重复，Value 可以重复（key 重复算一个，后添加会覆盖先添加的值）
    >
    >实现类: HashMap(散列表算法实现)
    >
    >TreeMap(二叉排序树实现,利用 Key 排序)
    >
    >Map 适合检查查找
- HashMap与HashTable的区别 http://www.importnew.com/7010.html
- HashMap与HashSet的关系:http://www.importnew.com/6931.html hashSet是由hashmap实现的
- HashSet的原理：http://www.importnew.com/19208.html
- ArrayList的用法 https://www.cnblogs.com/kungfupanda/p/7357142.html
- List、Set和Map的继承关系  https://www.cnblogs.com/jing99/p/7057245.html
- Collection 和 Collections的区别 http://pengcqu.iteye.com/blog/492196
- 其他集合类

#### 继承和接口

- interface和abstrat class抽象类的意义与区别:http://www.i3geek.com/archives/1230
- 实现接口，继承类的规则（单继承多实现）  
    >类可以一次实现多个接口，但是extends后面只能跟1个类，单继承，但是可以 B extends A， C extends B，这样也相当于 C  extends A,{}
- 接口继承接口
- 继承多个抽象类？ 
    >单继承  
- Overload和Override的区别。Overloaded的方法是否可以改变返回值的类型?
    >overload与override的区别 ... 重写(Overriding)是父类与子类之间多态性的一种表现，而重载(Overloading)是一个类中多态性的一种表现。 如果在子类中定义某方法与其父类有相同的名称和参数，我们说该方法被重写(Overriding)。  
- 对String类的继承
    > 不可以，因为String类有final修饰符，而final修饰的类是不能被继承的，实现细节不允许改变.  
    public final class String implements java.io.Serializable, Comparable<String>, CharSequence  
- abstract的method是否可同时是static,是否可同时是native，是否可同时是synchronized https://blog.csdn.net/fhm727/article/details/5222965
    >总体来说是都不能， abstract中的方法都是抽象出来的，只有被实现后才能被调用，而 static/native/synchronized表明该方法都是可以直接被使用的，与abstract矛盾。  
- 构造器Constructor是否可被override? 
    >Constructor(构造器)不能被继承，所以不能被override(重写)，但是可以被overloading(重载)。  

#### 异常处理

- Error、Exception和RuntimeException的区别，作用又是什么？列举3个以上的RuntimeException
    >https://blog.csdn.net/kwu_ganymede/article/details/51382461
    ```JAVA中常见的几种RuntimeException,大约有如下几种：
    NullPointerException - 空指针引用异常
    ClassCastException - 类型强制转换异常。
    IllegalArgumentException - 传递非法参数异常。
    ArithmeticException - 算术运算异常
    ArrayStoreException - 向数组中存放与声明类型不兼容对象异常
    IndexOutOfBoundsException - 下标越界异常
    NegativeArraySizeException - 创建一个大小为负数的数组错误异常
    NumberFormatException - 数字格式异常
    SecurityException - 安全异常
    UnsupportedOperationException - 不支持的操作异常```
- Java中的异常处理机制的简单原理和应用
    >https://blog.csdn.net/JavaReact/article/details/74910520
- 内存溢出和内存泄露
    >https://blog.csdn.net/buutterfly/article/details/6617375

#### 管道流

- inputStream和outputStream
    >https://blog.csdn.net/wangbaochu/article/details/53484042
- reader和inputstream
    >https://blog.csdn.net/xiadasong007/article/details/4776913
- Input/OutputStream和Reader/Writer有的区别
    >https://blog.csdn.net/u013087513/article/details/51915858
- 理解字符和字节
    >https://blog.csdn.net/u011514810/article/details/50809052

#### 线程

- 线程的生命周期：http://www.i3geek.com/archives/859
- java线程池：http://www.i3geek.com/archives/823
- 对run和start方法的理解: https://blog.csdn.net/u014236541/article/details/50198683
- 线程同步的基本方法 https://www.cnblogs.com/XHJT/p/3897440.html
- 死锁的问题 https://www.ibm.com/developerworks/cn/java/j-lo-deadlock/index.html

#### 其他

- 四种引用，强引用、软引用、弱引用和虚引用 ：http://www.i3geek.com/archives/1239
- String与StringBuilder,StringBuffer的区别  https://blog.csdn.net/kingzone_2008/article/details/9220691
- StringBuffer的实现方式，容量扩充  https://blog.csdn.net/yeweiyang16/article/details/51755552
- 对于 String str ="1"+"2"; 产生了几个对象  
    >3个  
- equal与==的区别
    >==就看两边长的一不一样    
    equal看两边是否相同，比较的是地址，看内在
- hashCode的作用 https://blog.csdn.net/fenglibing/article/details/8905007
    
- 为什么重写equals就必须重写hashCode https://blog.csdn.net/javazejian/article/details/51348320
- 自动拆装箱：http://www.i3geek.com/archives/990
- NIO  
    >https://blog.csdn.net/u013256816/article/details/51457215  
    https://yq.aliyun.com/articles/2371  
- java动态代理
    >https://www.ibm.com/developerworks/cn/java/j-lo-proxy1/index.html  
    https://www.ibm.com/developerworks/cn/java/j-lo-proxy2/index.html
    http://www.importnew.com/27772.html
    
- 序列化与反序列化 http://www.infoq.com/cn/articles/serialization-and-deserialization
- public、protected、private以及默认的作用域 https://blog.csdn.net/qq_31686787/article/details/52553974
- Object类的学习和理解，基本的方法 
    >https://blog.csdn.net/a724888/article/details/80153002  
    http://www.cnblogs.com/binyue/p/3434918.html
- char类型的大小，对汉字的存储  https://blog.csdn.net/u010361662/article/details/56510077
- java中传值和传引用的理解，四种引用  http://www.cnblogs.com/binyue/p/3862276.html
- 正则表达式

### Java进阶

#### 多线程

- 多线程要注意什么？  
    >https://blog.csdn.net/kkgbn/article/details/56279659  
     https://www.jianshu.com/p/da705fad8400  
- volatile的关键字学习  https://blog.csdn.net/u010255818/article/details/65633033
- 多线程保证同步的所有方法，除了synchronized外还有什么？  https://blog.csdn.net/kingcat666/article/details/75675955
- java中sleep和wait的区别：http://www.i3geek.com/archives/1173
- 理解和使用wait/notify
    >https://blog.csdn.net/wthfeng/article/details/78762343  
    http://www.importnew.com/16453.html
- 守护线程的含义  https://blog.csdn.net/lcore/article/details/12280027
- 正确的停止一个线程   https://www.cnblogs.com/greta/p/5624839.html
- 对synchronized的理解，锁的是什么？锁静态方法和非静态方法的区别  https://blog.csdn.net/u010842515/article/details/65443084/

#### 虚拟机

##### 内存结构
- 虚拟机的内存结构，堆内存、栈内存、方法区、常量池等：http://www.i3geek.com/archives/1201
- JVM中的内存设置和分配：http://www.i3geek.com/archives/1138
- 分别存储什么，对象和基本成员变量的存储区域  https://www.cnblogs.com/wangjzh/p/5258254.html  

##### GC垃圾回收   
- gc的概念，什么需要回收？  https://blog.csdn.net/oopsoom/article/details/40348125  
- 怎么判断被回收？有哪些方法  https://segmentfault.com/a/1190000008764361
- 引用计数方法，对象引用遍历和分代回收方法是什么  https://www.cnblogs.com/laoyangHJ/articles/java_gc.html
- 怎么避免对象循环引用的回收  https://www.cnblogs.com/lihaozy/archive/2013/06/08/3125974.html
- Java中的内存溢出是如何造成的：http://www.i3geek.com/archives/1241
- Java中的内存溢出和C＋＋中的内存溢出，是一个概念吗？：http://www.i3geek.com/archives/1241

    >http://www.i3geek.com/archives/1220    
    
    
##### CLASSLOADER

- 什么是类加载器
- 哪三层类加载器
- 什么加载顺序
- 功能是什么？工作模式是什么？
- 项目中的例子，加载必要jar包
    >https://www.ibm.com/developerworks/cn/java/j-lo-classloader/index.html  
    https://blog.csdn.net/xyang81/article/details/7292380  
- 反射的原理，什么是反射？  http://www.importnew.com/23902.html
- 反射的运用，反射是否可以调用私有方法 http://wiki.jikexueyuan.com/project/java-reflection/java-private.html
    
      
    
    

#### 其他

- NIO是什么  
    >https://www.ibm.com/developerworks/cn/education/java/j-nio/j-nio.html  
    http://wiki.jikexueyuan.com/project/java-nio/nio-io.html
- PRC远程服务原理及作用：http://www.i3geek.com/archives/941
- JMS消息服务框架  https://www.ibm.com/developerworks/cn/java/wa-spring4/index.html
- io和nio的本质以及使用场景  https://blog.csdn.net/qq_35280514/article/details/77542158
- java 8的新特性
    >http://www.importnew.com/11908.html  
    https://www.ibm.com/developerworks/cn/java/j-lo-jdk8newfeature/index.html
- hashcode 有哪些算法  https://www.jianshu.com/p/bf1d7eee28d0
- 泛型的实现机制  https://www.ibm.com/developerworks/cn/java/j-jtp01255.html         
- Socket编程通常出现的异常有哪些，什么情况下会出现  https://blog.csdn.net/qq_20889581/article/details/52402088
- 了解JVM启动参数 -verbose -Xms -Xmx的意思  https://www.ibm.com/support/knowledgecenter/zh/SSYKE2_8.0.0/com.ibm.java.vm.80.doc/docs/x_jvm_commands.html

### J2EE

#### 基本概念

- 分清javaEE、Tomcat、JVM等概念：http://www.i3geek.com/archives/848

#### Servlet

- servlet的基本概念   http://www.importnew.com/14621.html   http://www.importnew.com/14621.html
- servlet的生命周期  https://www.jianshu.com/p/1d5089a635af
- servlet中定制session的过期时间  https://blog.csdn.net/wzx735481897/article/details/54582228
- Servlet中的session工作原理 （禁用cookie如何使用session）  https://www.jianshu.com/p/395bac076ea9
- filter和listener是什么？有什么区别？servlet、filter、listener：http://www.i3geek.com/archives/870

#### Web框架

- MVC模型概念  https://blog.csdn.net/luxuejuncarl/article/details/1472185
- Spring IoC 中的BeanFactory：http://www.i3geek.com/archives/878
- Spring AOP 原理：http://www.i3geek.com/archives/912
- Spring的事务管理:   
    >https://blog.csdn.net/justloveyou_/article/details/73733278  
    https://www.jianshu.com/p/e063858d94f2
- Spring bean注入的几种方式  https://www.cnblogs.com/duanxz/p/4716720.html

# java面试(一线企业校招、社招)
>友情提示：下面面试题和技术难度，主要正对国内一线企业校招和社招，请量力而为，不要信心受挫。
>故，做为致力于一线企业校招的你来说，能把每个知识模块的一小部分问题去深入学习和总结，已经很棒了，加入BAT企业“随心所欲”！

## 基础   

- Arrays.sort实现原理和Collection实现原理   https://www.jianshu.com/p/4d8c6b8b9ede
    >在jdk7以前的版本中sort()的实现原理是:基本类型使用优化后的快速排序,其他类型使用优化后的归并排序,jdk7以后如果jdk7以后修改了排序策略:如果JVM启动参数配置了-Djava.util.Arrays.useLegacyMergeSort%3Dtrue+那么就会执行上面所说的排序策略(优化的归并排序),否则将会执行TimSort排序。&oq=在jdk7以前的版本中sort()的实现原理是:基本类型使用优化后的快速排序,其他类型使用优化后的归并排序,jdk7以后如果jdk7以后修改了排序策略:如果JVM启动参数配置了-Djava.util.Arrays.useLegacyMergeSort%3Dtrue++那么就会执行上面所说的排序策略(优化的归并排序),否则将会执行TimSort排序。事实上Collections.sort方法底层就是调用的array.sort方法  
- foreach和while的区别(编译之后)
    >foreach加强for循环，已知循环次数，逐条读取，一般用于对象集合。 while循环不确定循环次数，逐行读取。只要满足条件就一直循环下去。
     应用场景不同。
     foreach用于对数组、集合类进行循环处理，一个例子：
     ```
      int[] fibarray = new int[] { 0, 1, 1, 2, 3, 5, 8, 13 };
      foreach (int element in fibarray)
      {
          System.Console.WriteLine(element);
      }
     
     ```
             
     >while用于不确定循环次数的情况，一个例子：
     ```
     int i=0;
     while(i > 999){
        System.out.println(i);
        i = i+20;
     }
     ```
     >至于性能上的差距，因为和多个因素相关(循环体内是否定义使用局部变量，循环处理的数据结构等)。
     不能轻易的下结论谁优谁劣。
     不是对性能要求特别苛刻的场合，也不用过于在意。
   
- 线程池的种类，区别和使用场景
    >https://blog.csdn.net/w05980598/article/details/79425071  
     https://www.ibm.com/developerworks/cn/java/j-jtp0730/index.html
- 分析线程池的实现原理和线程的调度过程     
    >实现原理：https://blog.csdn.net/qq_34531925/article/details/73121455  
    调度过程：http://www.zhenchao.org/2017/08/31/java-thread-pool-executor/
- 线程池如何调优   
    >http://youyu4.iteye.com/blog/2400407  
    https://www.cnblogs.com/jianzh5/p/6437315.html
- 线程池的最大线程数目根据什么确定  
    >http://ifeve.com/how-to-calculate-threadpool-size/  
    >https://edagarli.gitbooks.io/java-route/content/
- 动态代理的几种方式   https://blog.csdn.net/heyutao007/article/details/49738887
- HashMap的并发问题   https://my.oschina.net/xianggao/blog/393990   
- 了解LinkedHashMap的应用吗  
    >https://blog.csdn.net/justloveyou_/article/details/71713781  
    https://yikun.github.io/2015/04/02/Java-LinkedHashMap%E5%B7%A5%E4%BD%9C%E5%8E%9F%E7%90%86%E5%8F%8A%E5%AE%9E%E7%8E%B0/
- 反射的原理，反射创建类实例的三种方式是什么？  https://www.cnblogs.com/ysw-go/p/5335948.html  
- cloneable接口实现原理，浅拷贝or深拷贝   
    >https://zhuanlan.zhihu.com/p/23999973  
    https://www.kancloud.cn/hx78/java/334807  
- hashtable和hashmap的区别及实现原理，hashmap会问到数组索引，hash碰撞怎么解决   
    >https://blog.csdn.net/u010983881/article/details/49762595  
    http://www.importnew.com/7010.html
    https://yikun.github.io/2015/04/01/Java-HashMap%E5%B7%A5%E4%BD%9C%E5%8E%9F%E7%90%86%E5%8F%8A%E5%AE%9E%E7%8E%B0/
    https://www.oschina.net/question/16_8758
    
- arraylist和linkedlist区别及实现原理   
    >http://www.importnew.com/6629.html  
    https://blog.csdn.net/eson_15/article/details/51145788
    
- 反射中，Class.forName和ClassLoader区别    https://www.jianshu.com/p/50e18a563301
- String，Stringbuffer，StringBuilder的区别？   https://www.jianshu.com/p/8c724dd28fa4
- 有没有可能2个不相等的对象有相同的hashcode   
    >有可能，所以两个对象比较的时候，先比较hashcode，然后在比较equals（）
- TreeMap的实现原理   https://www.ibm.com/developerworks/cn/java/j-lo-tree/index.html

### JVM相关   

- 类的实例化顺序，比如父类静态数据，构造函数，字段，子类静态数据，构造函数，字段，他们的执行顺序   
    > https://segmentfault.com/a/1190000004527951  
    https://blog.csdn.net/xiaoxuanfeng1986/article/details/46710979
    
- JVM内存分代   http://www.importnew.com/19255.html
- Java 8的内存分代改进   
    >http://caoyaojun1988-163-com.iteye.com/blog/1969853  
    https://www.jianshu.com/p/d23524a61079  
    https://blog.csdn.net/u012834750/article/details/70160594
    
- JVM垃圾回收机制，何时触发MinorGC等操作   
    >垃圾回收机制 https://www.ibm.com/developerworks/cn/java/j-lo-JVMGarbageCollection/index.html
    何时出发GC： https://blog.csdn.net/yhyr_ycy/article/details/52566105
- jvm中一次完整的GC流程（从ygc到fgc）是怎样的，重点讲讲对象如何晋升到老年代，几种主要的jvm参数等   https://blog.csdn.net/zd836614437/article/details/64126826
- 你知道哪几种垃圾收集器，各自的优缺点，重点讲下cms，g1   https://crowhawk.github.io/2017/08/15/jvm_3/
- 新生代和老生代的内存回收策略  http://www.360doc.com/content/12/1023/16/9615799_243296263.shtml 
- Eden和Survivor的比例分配等  https://blog.csdn.net/Muyundefeng/article/details/72667863  
- 深入分析了Classloader，双亲委派机制    https://blog.csdn.net/u011080472/article/details/51332866
- JVM的编译优化     https://www.jianshu.com/p/958a50db3c57
- 对Java内存模型的理解，以及其在并发中的应用     https://zhuanlan.zhihu.com/p/27361117
- 指令重排序，内存栅栏等    https://www.cnblogs.com/chenyangyao/p/5269622.html
- OOM错误，stackoverflow错误，permgen space错误   
- JVM常用参数   http://www.cnblogs.com/redcreen/archive/2011/05/04/2037057.html
- tomcat结构，类加载器流程    
    >https://www.cnblogs.com/xing901022/p/4574961.html
    http://wiki.jikexueyuan.com/project/tomcat/classloading.html
- volatile的语义，它修饰的变量一定线程安全吗    https://www.ibm.com/developerworks/cn/java/j-jtp06197.html
- g1和cms区别,吞吐量优先和响应优先的垃圾收集器选择    
- 说一说你对环境变量classpath的理解？如果一个类不在classpath下，为什么会抛出ClassNotFoundException异常，如果在不改变这个类路径的前期下，怎样才能正确加载这个类？   
- 说一下强引用、软引用、弱引用、虚引用以及他们之间和gc的关系     https://juejin.im/post/5b30a28df265da5967193a9c  

### JUC/并发相关   

- ThreadLocal用过么，原理是什么，用的时候要注意什么   https://blog.csdn.net/lufeng20/article/details/24314381
- Synchronized和Lock的区别   https://juejin.im/post/5a43ad786fb9a0450909cb5f
- synchronized 的原理，什么是自旋锁，偏向锁，轻量级锁，什么叫可重入锁，什么叫公平锁和非公平锁
    >https://blog.csdn.net/Kirito_j/article/details/79201213  <br>
        https://www.jianshu.com/p/6d9c0b5d2801
- concurrenthashmap具体实现及其原理，jdk8下的改版   http://www.jasongj.com/java/concurrenthashmap/
- 用过哪些原子类，他们的参数以及原理是什么    https://blog.csdn.net/jijianshuai/article/details/70853776
- cas是什么，他会产生什么问题（ABA问题的解决，如加入修改次数、版本号）   http://zouzls.github.io/2017/01/26/CAS%E5%8E%9F%E5%AD%90%E6%93%8D%E4%BD%9C/
- 如果让你实现一个并发安全的链表，你会怎么做   https://www.jianshu.com/p/377666236271 
- 简述ConcurrentLinkedQueue和LinkedBlockingQueue的用处和不同之处  
    >https://www.cnblogs.com/wzhanke/p/4763356.html<br> 
    阻塞队列：线程安全<br>
     按 FIFO（先进先出）排序元素。队列的头部是在队列中时间最长的元素。队列的尾部是在队列中时间最短的元素。新元素插入到队列的尾部，并且队列检索操作会获得位于队列头部的元素。链接队列的吞吐量通常要高于基于数组的队列，但是在大多数并发应用程序中，其可预知的性能要低。
     注意：<br>
     1、必须要使用take()方法在获取的时候达成阻塞结果<br>
     2、使用poll()方法将产生非阻塞效果<br>
     非阻塞队列<br>
     基于链接节点的、无界的、线程安全。此队列按照 FIFO（先进先出）原则对元素进行排序。队列的头部 是队列中时间最长的元素。队列的尾部 是队列中时间最短的元素。新的元素插入到队列的尾部，队列检索操作从队列头部获得元素。当许多线程共享访问一个公共 collection 时，ConcurrentLinkedQueue是一个恰当的选择。此队列不允许 null 元素。<br>
     在并发编程中，一般推荐使用阻塞队列，这样实现可以尽量地避免程序出现意外的错误。阻塞队列使用最经典的场景就是socket客户端数据的读取和解析，读取数据的线程不断将数据放入队列，然后解析线程不断从队列取数据解析。还有其他类似的场景，只要符合生产者-消费者模型的都可以使用阻塞队列。<br>
     使用非阻塞队列，虽然能即时返回结果（消费结果），但必须自行编码解决返回为空的情况处理（以及消费重试等问题）。另外他们都是线程安全的，不用考虑线程同步问题。<br>
     
- 简述AQS的实现原理   
    >https://juejin.im/post/5aeb07ab6fb9a07ac36350c8<br>
    https://juejin.im/entry/58e6f484ac502e006c2b6887
- countdowlatch和cyclicbarrier的用法，以及相互之间的差别?   
    >https://www.jianshu.com/p/bce9f156080f<br>
    https://www.jianshu.com/p/bce9f156080f
- concurrent包中使用过哪些类？分别说说使用在什么场景？为什么要使用？   <br>https://juejin.im/post/5a093ff551882531bb6c4ee3
- LockSupport工具   <br>https://www.jianshu.com/p/9677a754cf60
- Condition接口及其实现原理   <br>https://juejin.im/entry/59756e5051882566d86d8a5d
- Fork/Join框架的理解   <br>https://www.jianshu.com/p/6b9347a22fd1
- jdk8的parallelStream的理解   <br>https://www.jianshu.com/p/bd825cb89e00
- 分段锁的原理,锁力度减小的思考  <br>https://blog.csdn.net/rlnLo2pNEfx9c/article/details/79784983<br> https://www.jianshu.com/p/9c713de7bbdb 

## Spring   

- Spring AOP与IOC的实现原理   https://blog.csdn.net/luoshenfu001/article/details/5816408
- Spring的beanFactory和factoryBean的区别    https://blog.csdn.net/wangbiao007/article/details/53183764
- 为什么CGlib方式可以对接口实现代理？    https://blog.csdn.net/qq_27093465/article/details/53340513 
- RMI与代理模式   https://blog.csdn.net/qq717559128/article/details/28894895
- Spring的事务隔离级别，实现原理    https://blog.csdn.net/zhousenshan/article/details/78509250
- 对Spring的理解，非单例注入的原理？它的生命周期？循环注入的原理，aop的实现原理，说说aop中的几个术语，它们是怎么相互工作的？  
- Mybatis的底层实现原理     <br>https://www.jianshu.com/p/ec40a82cae28 <br>https://my.oschina.net/xianggao/blog/591482
- MVC框架原理，他们都是怎么做url路由的   http://www.cnblogs.com/killbug/p/3593059.html
- spring boot特性，优势，适用场景等   
- quartz和timer对比   <br>https://www.jianshu.com/p/369803e790d6 <br>https://zhuanlan.zhihu.com/p/24989832
- spring的controller是单例还是多例，怎么保证并发的安全   
    > spring的controller默认是单例,<br>
    最佳实践：<br>
    1、不要在controller中定义成员变量。<br>
    2、万一必须要定义一个非静态成员变量时候，则通过注解@Scope("prototype")，将其设置为多例模式<br>
    改为多例的（就是在class上面加一个@Scope("request")）：
## 分布式相关    

- Dubbo的底层实现原理和机制   https://www.jianshu.com/p/ad5bc07b1b3e
- 描述一个服务从发布到被消费的详细过程   
- 分布式系统怎么做服务治理   https://blog.csdn.net/suifeng3051/article/details/53992560
- 接口的幂等性的概念   https://blog.csdn.net/WANGYAN9110/article/details/70953273
- 消息中间件如何解决消息丢失问题      https://blog.csdn.net/u011393781/article/details/52688761
- Dubbo的服务请求失败怎么处理   
- 重连机制会不会造成错误     https://blog.csdn.net/java20150326/article/details/79978789
- 对分布式事务的理解     http://www.cnblogs.com/savorboard/p/distributed-system-transaction-consistency.html
- 如何实现负载均衡，有哪些算法可以实现？   https://www.jianshu.com/p/40e196414cfa
- Zookeeper的用途，选举的原理是什么？      https://blog.csdn.net/yinwenjie/article/details/47613309
- 数据的垂直拆分水平拆分。   https://blog.csdn.net/Jerome_s/article/details/52492616
- zookeeper原理和适用场景   
    > http://www.wuzesheng.com/?p=2609<br>https://www.jianshu.com/p/b5f99fdb1957<br>https://my.oschina.net/hejiula/blog/151346
- zookeeper watch机制   
    > https://blog.csdn.net/qianshangding0708/article/details/50084155<br>https://www.ibm.com/developerworks/cn/opensource/os-cn-apache-zookeeper-watcher/index.html
- redis/zk节点宕机如何处理    
- 分布式集群下如何做到唯一序列号   
    > https://tech.meituan.com/MT_Leaf.html<br>https://www.cnblogs.com/haoxinyue/p/5208136.html
- 如何做一个分布式锁   
    > https://www.jianshu.com/p/c2b4aa7a12f1<br>http://www.hollischuang.com/archives/1716<br>http://www.importnew.com/27477.html
- 用过哪些MQ，怎么用的，和其他mq比较有什么优缺点，MQ的连接是线程安全的吗   
    > https://mp.weixin.qq.com/s?__biz=MzI3NDAwNDUwNg%3D%3D&mid=2648307598&idx=1&sn=eeaa9d795ef6ba13368e7a76ca14bae7&scene=45#wechat_redirect
- MQ系统的数据如何保证不丢失   
- 列举出你能想到的数据库分库分表策略；分库分表后，如何解决全表查询的问题。   
    > https://blog.csdn.net/xlgen157387/article/details/53976153<br>
    https://my.oschina.net/stephenzhang/blog/650225<br>
    https://juejin.im/entry/591968f6a0bb9f005ff7af23<br>
    http://www.infoq.com/cn/articles/key-steps-and-likely-problems-of-split-table
    

## 算法&数据结构&设计模式   

- 海量url去重类问题（布隆过滤器）  https://www.jianshu.com/p/88c6ac4b38c8
- 数组和链表数据结构描述，各自的时间复杂度   https://blog.csdn.net/wangshihui512/article/details/9787699
- 二叉树遍历    https://blog.csdn.net/My_Jobs/article/details/43451187
- 快速排序   http://wiki.jikexueyuan.com/project/easy-learn-algorithm/fast-sort.html
- BTree相关的操作    https://blog.csdn.net/endlu/article/details/51720299
- 在工作中遇到过哪些设计模式，是如何应用的   
- hash算法的有哪几种，优缺点，使用场景   https://www.jianshu.com/p/bf1d7eee28d0
- 什么是一致性hash   
    > https://blog.csdn.net/cywosp/article/details/23397179<br>https://blog.csdn.net/lihao21/article/details/54193868
- paxos算法   https://www.jianshu.com/p/06a477a576bf
- 在装饰器模式和代理模式之间，你如何抉择，请结合自身实际情况聊聊   
- 代码重构的步骤和原因，如果理解重构到模式？    
    > https://zhuanlan.zhihu.com/p/24333137<br>http://www.infoq.com/cn/articles/clean-code-refactor

## 数据库   

- MySQL InnoDB存储的文件结构    https://www.cnblogs.com/benshan/archive/2013/01/08/2851714.html
- 索引树是如何维护的？    https://www.jianshu.com/p/1775b4ff123a
- 数据库自增主键可能的问题  
    > http://www.cnblogs.com/binyue/p/5393749.html<br>http://www.cnblogs.com/zhoujinyi/p/3433823.html<br>http://www.bkjia.com/Mysql/864266.html
- MySQL的几种优化   
    > https://blog.csdn.net/guodongCC322/article/details/55195195<br>https://www.zhihu.com/question/19719997<br>https://blog.csdn.net/u013474436/article/details/49908683
- mysql索引为什么使用B+树   
    > https://blog.csdn.net/bigtree_3721/article/details/73650601<br>https://blog.csdn.net/jijianshuai/article/details/79084860<br>https://www.jianshu.com/p/4dbbaaa200c4<br>https://www.kancloud.cn/kancloud/theory-of-mysql-index/41856
- 数据库锁表的相关处理   http://www.uml.org.cn/sjjm/201003301.asp
- 索引失效场景    
    > https://blog.csdn.net/pzqingchong/article/details/54696309<br>https://blog.csdn.net/xupeng874395012/article/details/72637379 
- 高并发下如何做到安全的修改同一行数据，乐观锁和悲观锁是什么，INNODB的行级锁有哪2种，解释其含义   
    > https://blog.csdn.net/wgy8283335/article/details/79281197  <br>https://www.jianshu.com/p/f5ff017db62a<br>http://www.hollischuang.com/archives/914
- 数据库会死锁吗，举一个死锁的例子，mysql怎么解决死锁     
    > https://www.cnblogs.com/LBSer/p/5183300.html<br>https://blog.csdn.net/qq_16681169/article/details/74784193

## Redis&缓存相关   

- Redis的并发竞争问题如何解决?了解Redis事务的CAS操作吗   
    >http://www.cnblogs.com/iforever/p/5796902.html<br>http://www.cnblogs.com/iforever/p/5796902.html<br>http://fivezh.github.io/2017/05/24/Redis-cas/
- 缓存机器增删如何对系统影响最小，一致性哈希的实现   
- Redis持久化的几种方式，优缺点是什么，怎么实现的   https://www.jianshu.com/p/bedec93e5a7b
- Redis的缓存失效策略    
    > http://www.cnblogs.com/binyue/p/3726842.html<br>https://blog.csdn.net/xiangnan129/article/details/54928672
- 缓存穿透的解决办法   https://blog.csdn.net/zeb_perfect/article/details/54135506
- redis集群，高可用，原理   
    >https://blog.csdn.net/u010739551/article/details/55252441<br>  https://blog.csdn.net/qq_41849945/article/details/80821303 <br>https://blog.csdn.net/hayre/article/details/78822979 
- mySQL里有2000w数据，redis中只存20w的数据，如何保证redis中的数据都是热点数据   
    > https://blog.csdn.net/rechel0937/article/details/77715286 <br> https://segmentfault.com/q/1010000005664664
- 用Redis和任意语言实现一段恶意登录保护的代码，限制1小时内每用户Id最多只能登录5次   
    ```
           @Test
           public void loginTest2(){
               String key = "用户id";
               for(int i=0;i<5;i++){
                   long size = redisTemplate.opsForList().size(key);
                   if(size<=5){
                       redisTemplate.opsForList().rightPush(key,System.currentTimeMillis()+"");
                   }else{
                       List<String> t = redisTemplate.opsForList().range(key,0,size);
                       Long now = System.currentTimeMillis();
                       if(now-Long.valueOf(t.get(0))>30000){//三十秒内
                           redisTemplate.opsForList().leftPop(key);
                           redisTemplate.opsForList().rightPush(key,System.currentTimeMillis()+"");
                           //登录成功
                       }else{
                           //登录失败
                           System.out.print("一小时内不能登录超过五次");
                       }
                   }
               }

    ```
- redis的数据淘汰策略   http://wiki.jikexueyuan.com/project/redis/data-elimination-mechanism.html

## 网络相关   

- http1.0和http1.1有什么区别    https://blog.csdn.net/hguisu/article/details/8608888
- TCP/IP协议   https://zh.wikipedia.org/wiki/TCP/IP%E5%8D%8F%E8%AE%AE%E6%97%8F
- TCP三次握手和四次挥手的流程，为什么断开连接要4次,如果握手只有两次，会出现什么   
    > https://github.com/jawil/blog/issues/14
    `我们知道，3次握手完成两个重要的功能，既要双方做好发送数据的准备工作(双方都知道彼此已准备好)，也要允许双方就初始序列号进行协商，这个序列号在握手过程中被发送和确认。
         现在把三次握手改成仅需要两次握手，死锁是可能发生的。作为例子，考虑计算机S和C之间的通信，假定C给S发送一个连接请求分组，S收到了这个分组，并发 送了确认应答分组。按照两次握手的协定，S认为连接已经成功地建立了，可以开始发送数据分组。可是，C在S的应答分组在传输中被丢失的情况下，将不知道S 是否已准备好，不知道S建立什么样的序列号，C甚至怀疑S是否收到自己的连接请求分组。在这种情况下，C认为连接还未建立成功，将忽略S发来的任何数据分 组，只等待连接确认应答分组。而S在发出的分组超时后，重复发送同样的分组。这样就形成了死锁。`
- TIME_WAIT和CLOSE_WAIT的区别   https://blog.csdn.net/kobejayandy/article/details/17655739
- 说说你知道的几种HTTP响应码   
- 当你用浏览器打开一个链接的时候，计算机做了哪些工作步骤   https://www.zhihu.com/question/34873227
- TCP/IP如何保证可靠性，数据包有哪些数据组成    
    > https://juejin.im/post/598ba1d06fb9a03c4d6464ab<br>https://blog.csdn.net/FX677588/article/details/76652236
- 长连接与短连接  http://www.cnblogs.com/0201zcr/p/4694945.html   
- Http请求get和post的区别以及数据包格式   https://blog.csdn.net/wuhuagu_wuhuaguo/article/details/63252447
- 简述tcp建立连接3次握手，和断开连接4次握手的过程；关闭连接时，出现TIMEWAIT过多是由什么原因引起，是出现在主动断开方还是被动断开方。    

## 其他  

- maven解决依赖冲突,快照版和发行版的区别   https://blog.csdn.net/wangb_java/article/details/66000956
- Linux下IO模型有几种，各自的含义是什么  https://www.jianshu.com/p/486b0965c296
- 实际场景问题，海量登录日志如何排序和处理SQL操作，主要是索引和聚合函数的应用   
    >分而治之:<br> https://blog.csdn.net/gogokongyin/article/details/51303868<br>https://segmentfault.com/q/1010000007402947
- 实际场景问题解决，典型的TOP K问题   
- 线上bug处理流程   
- 如何从线上日志发现问题    
- linux利用哪些命令，查找哪里出了问题（例如io密集任务，cpu过度）   
- 场景问题，有一个第三方接口，有很多个线程去调用获取数据，现在规定每秒钟最多有10个线程同时调用它，如何做到。   
    >https://zhuanlan.zhihu.com/p/20872901  
    http://blog.didispace.com/spring-boot-request-limit/    
- 用三个线程按顺序循环打印abc三个字母，比如abcabcabc。   
- 常见的缓存策略有哪些，你们项目中用到了什么缓存系统，如何设计的   
- 设计一个秒杀系统，30分钟没付款就自动关闭交易（并发会很高）   
- 请列出你所了解的性能测试工具   
- 后台系统怎么防止请求重复提交？   
- 有多个相同的接口，我想客户端同时请求，然后只需要在第一个请求返回结果的时候返回给客户端     



好的网站：
http://www.jasongj.com/
