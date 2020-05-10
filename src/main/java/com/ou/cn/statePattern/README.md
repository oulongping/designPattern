
# 描述

## 状态模式：

    允许一个对象在其内部状态改变是，改变它的行为，对象看起来似乎修改了它的类
    
    引自GOF所著《Design Patterns》
    
    状态模式的结构中包含三种角色
    1.环境（Context）：环境是一个类，该类含有抽象状态（State）声明的变量，可以引用任何具体状态类的实例，用户对该环境类(Context)类的
      实例在某种状态下的行为感兴趣
    2.抽象状态（State）： 抽象状态是一个接口或抽象类，抽象状态中定义了与环境(Context)的一个特定状态相关的若干个方法
    3.具体状态(Concrete State): 具体状态是实现抽象状态的类

### 使用场景：
    一个对象的行为依赖于它的状态，并且他必须在运行时根据状态的改变它的行为；需要编写大量的条件分支语句来决定一个操作的行为，而且这些条件
    恰好表示对象的一种状态。假设我们现在要设计一个带文字提示的温度计，可以根据用户的需求显示某些提示信息，比如用户希望温度在0度以下时，
    显示提示信息为"低温温度"，温度在10-26时，提示"温度正常"，当温度大于38时，提示"高温温度"
    
    下面，我们就以刚才说的温度计为例进行阐述说明。