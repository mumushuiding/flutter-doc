## 语法

基本的语法骨架是java

### ?? 的使用

```
// 如果a不为空, x等于a,否则x等于b
var x = a ?? b
```

### Key 的使用

当使用Stateful Widget时，集合内有数据移动和改变并且需要展示到界面时才需要key。

Stateful组件发生变化时，flutter会检查元素的Type和Key，如果没有Key,而Type未发生变化，则不会重新渲染;如果有Key，且发生变化，则flutter会重新渲染变化的组件

### PageStorageKey的使用

从一个页面进入另一个页面，返回时还是保留着跳转前的最后的状态，可以使用PageStorageKey、PageStorageBucket和PageStorage这几个类

### 借鉴C++语言

#### construct 

借鉴了C++语言的默认值使用以及使用冒号快速赋值法

#### typedef

类型定义：

```
typedef Callback = void Function();
```

### var 关键词的使用

借鉴了js语言，可以使用var关键词

### 同java的不同之处

1、new 关键词： 可用可不用，效果上没有区别

## 库

### shared_preferences

SharedPreferences轻量级存储类，以键值对的形式保存设置，属性和数据。

## 类

### AutomaticKeepAliveClientMixin 页面缓存

让页面一直保存在内存中不被销毁

### BoxDecoration 边框

添加下边框

```
Container(
      decoration: BoxDecoration(
        border: Border(bottom: BorderSide(width: 1,color: Colors.grey)),
      ),
    );
```


### double

#### infinity
```
// 强制在宽度上撑满
width: double.infinity
```

### SliverGrid

一行显示两个或者多个

### Stack 组件堆叠

可以将组件一层层堆叠起来


### StatefulWidget 

#### dispose 方法

Flutter的对象销毁机制同C++类似，所以很容易出现内存泄露问题，需要合理使用dispose销毁自己创建的对象