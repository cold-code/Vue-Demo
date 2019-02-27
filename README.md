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

