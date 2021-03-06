
# 描述

## 生成器模式：

    将一个复杂对象的构建与它的表示分离，使同样的过程可以创建不同的表示
    
    引自GOF所著《Design Patterns》
    
    生成器模式（也称建造者模式）的结构中包含四种角色
    1.产品（Product）：具体生成器要构造的复杂对象
    2.抽象生成器（Builder）： 抽象生成器是一个接口，该接口除了为创建一个Product对象的各个组件定义了若干个方法外，还定义了返回Product
      的方法
    3.具体生成器(ConcreteBuilder): 实现抽象生成器接口的类，具体生成器将实现Builder接口所定义的方法
      行适配。
    4.指挥者（Director）：指挥者是一个类，该类需包含有Builder接口声明的变量，指挥者的职责是负责向用户提供具体生成器，即指挥者将请求具
      体生成器来构造用户所需要的Product对象，如果所请求的具体生成器成功的构造出Product对象，指挥者就可以让具体生成器返回所狗仔的
      Prodcut对象

### 使用场景：
    当系统准备为用户提供一个内部结构复杂的对象，而且在构造方法中编写创建该对象的代码无法满足用户需求时，就可以用生成器模式来构造这样的
    对象；当某些系统请求对象的构造过程必须独立于创建该对象的类时。比如现在有某种商品，由于属性很多，用平实我们的构造器或者setter方法，
    会造成我们客户端的代码繁杂凌乱。这时候，就可以用生成器模式，减少客户端的这种重复代码。
    
    下面，我们就以刚才说的生成某件商品对象为例进行阐述说明。