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
