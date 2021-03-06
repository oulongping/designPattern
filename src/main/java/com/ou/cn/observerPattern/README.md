
# 描述

## 观察者模式：

    定义对象间的一种一对多的依赖关系，当一个对象的状态发生变化时，所有依赖它的对象都得到通知并被自动更新
    
    引自GOF所著《Design Patterns》
    
    观察者模式的结构中包含四种角色
    1.主题：主要是定义接口，规定具体主题需要实现的基本方法
    2.观察者： 主要是定义接口，规定具体的观察者需要实现的基本方法
    3.具体主题: 主要实现主题接口，包含可以经常变化的数据，并且有个集合，用来存放观察者，以便数据变化时通知具体观察者
    4.具体观察者： 主要实现观察者接口, 接收订阅的信息

### 使用场景：
    涉及多个对象都对一个特殊对象中的数据变化敢兴趣，而且这多个对象都希望跟踪那个特殊对象中的数据变化。例如我们公司有个微信群，公司的每个
    人都关心微信群里的信息变化，那如果某个员工想知道群里的信息变化，那么他就必须加入这个群，这样，每次群里有新的信息，就会及时通知他最新
    的消息，那如果哪天这个员工离职了，也就不在关心群里的信息了，那么退出群之后，就不会再收到信息了。
    
    下面，我们就以刚才说的公司微信群为例进行阐述说明(观察者模式也可以灵活设计，不一定要跟我的例子一样)。