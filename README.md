# Vue-Demo
## Part 1 Vue test demo

[Hello World demo](#)

[V-if & v-else & v-show demo](#)

[v-for demo](#)

[v-text demo](#)

[v-on demo](#)  
踩坑纪实：对于直接操作构造器内data数据的组件应该位于app容器内，除非使用Vue.extend扩展实例构造器或者用原生函数绑定事件调用Vue.set(el,key,value)来修改数据

[v-model demo](#)

[v-bind demo](#)

[v-pre & v-cloak & v-once demo](#)

## Part 2 Vue public API demo

[Vue.directive demo](#)  
踩坑纪实：el.style = "color:"+binding.value 的写法在IE浏览器无效  可替换成el.style.color = binding.value的写法

[Vue.extend demo](#)

[Vue.set demo](#)

[lifecycle（生命周期） demo](#)

[Vue template demo](#)  
踩坑纪实：IE暂不支持Template模板

[Vue component-1 组件（1）demo](#)  
笔记：定义局部组件时，组件名一定要是字符串类型

[Vue component-2 组件（2）demo](#)  
笔记：定义局部组件时，自定义属性注册props为数组类型，props内的属性值遇到'-'用小驼峰代替；  
踩坑纪实：给自定义属性绑定值时应该用的构造器内data选项里面的值;

[Vue component-3 组件（3）demo](#)  
笔记：子组件一定要在父组件引用之前声明；

[Vue component-4 组件（4）demo](#)  

## Part 3 Vue options demo

[Vue propsData Option demo](#) 

[Vue computed Option demo](#)  
笔记：数组倒序重排 arr.reverse()  
踩坑纪实：在computed下方法内用到构造器data内的参数得加this引用

[Vue methods Option demo](#)   
笔记：四种常见用法：  
1.传参用法；  
2.$event鼠标属性参数;  
3.自定义组件借用.native修饰器来调用构造器里methods选项内的方法；  
4.外部组件用原生onclick事件调取app.add()方法；（不建议,应该合理组织代码避免这类用法）

[Vue watch Option demo](#)  
笔记：可以在构造器外部用app.$watch的方法实施监控

[Vue Mixins Option demo](#)  
笔记：调用顺序全局 => 构造器 => 原生钩子  
踩坑纪实：全局调用mixin不加s

[Vue Extends Option && Delimiters Option demo](#)  
笔记: 扩展内的同名methods方法无效  
踩坑纪实：扩展选项只能赋值一个扩展对象，而mixins可以是多个对象组成的数组

## Part 4 Example Methods demo

[Vue Example1 Methods Demo](#)  
笔记：若引入了jQuery库就只能在mounted挂载了Dom结构后才能用jQuery来操作Dom

[Vue Example2 Methods Demo](#)  
笔记：nextTick方法的执行是在回调函数中进行，区别于destroy，reload

[Vue Example3 Methods Demo](#)  
笔记：在构造器外部添加进构造器内部的方法xx，需要在构造器外部用$emit(xx)调用一下  

[Vue Example3 Methods Demo](#)  
踩坑纪实：  
1.components一定要放在和构造器内data选项同级的位置；  
2.如果要在组件内调用构造器内的方法应该放在自定义组件内调用而不是template内调用，调用时加'()'执行；
