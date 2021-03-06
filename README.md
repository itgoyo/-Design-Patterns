# Design-Patterns

# 设计模式

## 设计模式的原则
- 单一职责原则
- 接口隔离原则
- 依赖倒转原则
- 里氏替换原则
- 开闭原则
- 迪米特法则
- 合成复用原则

- 单一职责原则
	- 摩托车
	- 飞机
	- 轮船


- 接口隔离原则
	- 可以写多个接口，然后需要的直接继承即可 即一个类对另一个类的依赖简历在最小的接口上 大的接口拆开成小的接口，我只需要继承小的即可
	
- 依赖倒转原则
	- 高层依赖不应该依赖底层的模块，二者都应该依赖其抽象
	- 抽象不应该依赖细节，细节应该依赖抽象
	- 依赖倒转的中心思想是面向接口编程
	- 设计理念：相对于细节的多变性，抽象的东西要稳定的多。以抽象为基础搭建的架构比细节为基础的架构要稳定的多，在Java中，抽象指的是接口或者是抽象类，细节就是具体的实现类
	- 使用接口或者抽象类的目的是制定好规范，而不涉及任何具体的操作，把展现细节的任务交给他们的实现类去完成
### 依赖关系传递的三种方式：
- 接口传递
- 构造方法传递
- setter方式传递

- 里氏替换原则
	- 通常做法是：原来的父类和子类都继承一个更加通俗的基类，原有的继承关系去掉，采用依赖，聚合，组合等关系替代

- 开闭原则
	- 开闭原则是编程中最基础、最为中号的设计原则
	- 一个软件实体类，模块和函数应该对拓展开放（对提供方），对修改关闭（对使用仿）。用抽象构建框架，用实现拓展细节
	- 当软件需要变化时，尽量通过拓展软件实体的行为来实现变化，而不是通过修改已有的代码来实现变化
	-  编程中遵循其他软件，以及使用设计模式的目的就是遵循开闭原则

- 迪米特法则
	- 一个对象应该对其他对象保持最少的了解
	- 类与类关系越密切，耦合度越大
	- 迪米特法则又叫最少知道原则，即一个类对自己依赖的类知道的越少越好。也就是说对于被依赖的类不管多么复杂，都尽量将逻辑封装在类的内部。对外除了提供的public方法，不对外泄露任何信息
	- 迪米特法则还有一个更简单的定义：只与直接的朋友通信
	- **直接的朋友**：每个对象都会与其他对象有耦合关系，只要两个对象之间有耦合关系，我们就说这两个对象之间是朋友关系。耦合的方式很多，依赖，关联，组合，聚合等。其中我们称出现成员变量，方法参数，方法返回值中的类为直接朋友，而出现在局部变量中的类不是直接的朋友。也就是说，陌生的类最好不要以局部变量的形式出现在类的内部。

- 合成复用原则
	- 原则是尽量使用合成/聚合的方式，而不是使用继承

![](https://gitee.com/itgoyo/PicGoRes/raw/master/img/设计模式.png) 
 
# UML --Unified modeling language (统一建模语言)
- Note 注释
- Class 表示类，可以添加属性和方法
- Interface 表示接口
- Denpendency 表示依赖
- Association 表示关联
- Generalization 表示泛化（继承）
- Realization 表示实现
- Aggregation 表示聚合
- Composite 组合

![](https://gitee.com/itgoyo/PicGoRes/raw/master/img/20200516102048.png)
 

# 23种设计模式
 ![](https://gitee.com/itgoyo/PicGoRes/raw/master/img/20200516111410.png)

 - 创建型
	- 工厂方法模式 (Factory Method Pattern)
	- 抽象工厂模式 (Abstract Factory Pattern)
	- 单例模式 (Singleton Pattern)
	- 建造者模式 (Builder Pattern)
	- 原型模式 (Prototype Pattern)

 - 结构型
	- 适配器模式 (Adapter Pattern)
	- 装饰者模式 (Decorator Pattern)
	- 代理模式 (Proxy Pattern）
	- 外观模式 (Facade Pattern)
	- 桥接模式 (Bridge Pattern)
	- 组合模式 (Composite Pattern)
	- 享元模式 (Flyweight Pattern)

 - 行为型
	- 策略模式 (Strategy Pattern）
	- 模板方法模式 (Template Method Pattern）
	- 观察者模式 (Observer Pattern)
	- 迭代器模式 (Iterator Pattern)
	- 责任链模式 (Chain of Responsibility Pattern)
	- 命令模式 (Command Pattern)
	- 备忘录模式 (Memento Pattern)
	- 状态模式 (State Pattern)
	- 访问者模式 (Visitor Pattern)
	- 中介者模式 (Mediator Pattern)
	- 解释器模式 (Interpreter Pattern)

 设计模式的本质 **提高软件的维护性，通用性和拓展性，并降低软件的复杂度**