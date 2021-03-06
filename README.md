# designPattern

# java常见的设计模式

    已经工作了快5年时间了，一直没有好好的整理一下自己的思绪，很多知识都不成体系，有时候也只停留在会使用的层面上，没有深入的了解一些基本
    原理，越来越感觉到自己的掌握的知识浮于表面。所以下定决心用一年的时间，多深入了解一些技术知识的背后运行原理和使用场景，也算是对自己的
    一种鞭策，突破自己的瓶颈，所以就打算先从设计模式开始。设计模式是一套被反复使用的、多数人知晓的、经过分类编目的、代码设计经验的总结。
    
    熟练掌握各种设计模式，并能在实际编程开发中灵活运用它们，不仅能使代码更优雅，可扩展性强，同时也能保证代码的可靠性和可读性，对于后期
    的代码维护好处良多。设计模式于己于他人于系统都是多赢的，对于一个有经验的程序员来说，掌握并运用设计模式，是最基本的一项技能。
    
    **_欢迎各位同行进行交流哈_**
    
    顺便说明一下，以下七大设计原则，主要是摘录这篇博文。这种概念性的东西，鉴于水平有限，没有能力自己总结，还望谅解。
    
    https://www.jianshu.com/p/8a293e4a888e

## 七大设计原则

    面向对象编程有七大原则，提倡它的根本原因是为了代码复用，增加可维护性。设计模式就是实现了这些原则，从而达到了代码复用、增加可维护性的
    目的。因为设计模式就是基于这些原则的实现，所以很有必要了解这些原则，这也有助于我们对设计模式的理解，下面主要对面向对象编程的几个原则
    进行简单介绍。

### 1、单一职责原则 ( SRP )

    英文全称是Single Responsibility Principle，定义是一个类或者方法，应该只有一个引起它变化的原因。类变化的原因就是职责，如果一个类
    承担的职责过多，就等于把这些职责耦合在一起了。一个职责的变化可能会削弱或者抑制这个类完成其他职责的能力。这种耦合会导致脆弱的设计，当
    发生变化时，设计会遭受到意想不到的破坏。而如果想要避免这种现象的发生，就要尽可能的遵守单一职责原则。此原则的核心就是解耦和增强内聚性。

### 2、开闭原则 ( OCP )

    英文全称是Open Close Principle，定义是软件实体（包括类、模块、函数等）应该对于扩展时开放的，对于修改是封闭的。开闭原则是是面向
    对象设计中最重要的原则之一，其它很多的设计原则都是实现开闭原则的一种手段。

### 3、里氏替换原则 ( LSP )

    英文全称是Liskov Substitution Principle，是面向对象设计的基本原则之一。 定义是任何基类可以出现的地方，子类一定可以出现。LSP 是
    继承复用的基石，只有当派生类可以替换掉基类，且软件单位的功能不受到影响时，基类才能真正被复用，而派生类也能够在基类的基础上增加新的行
    为。里氏替换原则是对开闭原则的补充。实现开闭原则的关键步骤就是抽象化，而基类与子类的继承关系就是抽象化的具体实现，所以里氏替换原则是
    对实现抽象化的具体步骤的规范。

### 4、依赖倒置原则 ( DIP )

    英文全称是Dependence Inversion Principle，这个原则是开闭原则的基础，依赖倒置原则就是要求调用者和被调用者都依赖抽象，这样两者没
    有直接的关联和接触，在变动的时候，一方的变动不会影响另一方的变动。依赖倒置强调了抽象的重要性，针对接口编程，依赖于抽象而不依赖于具体。

### 5、接口隔离原则 ( ISP )

    英文全称是Interface Segregation Principle，这个原则的意思是使用多个隔离的接口，比使用单个接口要好。目的就是降低类之间的耦合度，
    便于软件升级和维护。

### 6、最少知道原则(迪米特原则)

    一个实体应当尽量少地与其他实体之间发生相互作用，使得系统功能模块相对独立。通俗地说就是不要和陌生人说话，即一个对象应对其他对象有尽
    可能少的了解。迪米特法则的初衷在于降低类之间的耦合。由于每个类尽量减少对其他类的依赖，因此，很容易使得系统的功能模块功能独立，相互之
    间不存在（或很少有）依赖关系。

### 7、合成/聚合复用（CARP）

    英文全称是Composite Reuse Principle，合成/聚合复用原则经常又叫做合成复用原则。合成/聚合复用原则的潜台词是：我只是用你的方法，我
    们不一定是同类。继承的耦合性更大，比如一个父类后来添加实现一个接口或者去掉一个接口，那子类可能会遭到毁灭性的编译错误，但如果只是组合
    聚合，只是引用类的方法，就不会有这种巨大的风险，同时也实现了复用。

    我们的设计模式基本都是围绕这些原则来设计的，不同的业务场景，可以用不同的设计模式。
    
    但是切记，每种设计模式都有不同的写法，所以有不一样的时候，不用惊讶，要学会灵活运用。

作者：夏林梦子

链接：https://github.com/LongpingOu/designPattern