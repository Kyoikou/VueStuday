# 简单认识一下Vue.js

读音(vju)

- 渐进式框架
- Web开发高级功能：
  - 解耦视图和数据
  - 可复用的组件
  - 前端路由技术
  - 状态关联
  - 虚拟DOM

## 1、Vue初体验

```html
<div id="app">

</div>

<script src="../js/vue.js"></script>
<script>
    // let(变量)/ const(常量)
    const app = new Vue({
        el: '#app'
    })
</script>
```

> new Vue()
>
> vue.js里面一定用一个 function Vue  且传参为对象类型
>
> ```html
> <!-- vue.js-->
> <script> 
> 	function Vue({...}){
>         
>     }
> </script>
> ```
>
> 

> el: '#app'  ：定义要挂载的元素

> 编程范式：**声明式编程**
>
> ```html
> {{message}}
> 
> data: {
>                 message: '你还啊啊啊'
> }
> ```
>
> ```console
> app.message = '控制台直接改'
> ```
>
> 

**请看代码的三个小案例  vuelearn01 - 03**

## 2、MVVM

看维基百科

![image-20201108174757724](C:\Users\今天以后\AppData\Roaming\Typora\typora-user-images\image-20201108174757724.png)

![image-20201108174927342](C:\Users\今天以后\AppData\Roaming\Typora\typora-user-images\image-20201108174927342.png)

## 3、创建Vue实例传入的option

![image-20201108175420624](C:\Users\今天以后\AppData\Roaming\Typora\typora-user-images\image-20201108175420624.png)

> el 
>
> - String:'#app'
>
> - HTML Element
>
> method（方法）:
>
> - 方法叫methods
>
> - 函数 function
>
> - > 方法跟函数有什么区别？
>   >
>   > 方法是面向对象的，函数可以说是面向过程
>   >
>   > **函数** 是写在外边
>   >
>   > ```html
>   > <script>
>   >     function qqq(){
>   >         
>   >     }
>   > </script>
>   > ```
>   >
>   > **方法** 是写在类里面，**一定要与实例对象挂钩！**
>   >
>   > ```js
>   > function Person(){
>   >     method1: function(){
>   >         
>   >     }
>   > }
>   > ```
>   >
>   > 

![image-20201108175458482](C:\Users\今天以后\AppData\Roaming\Typora\typora-user-images\image-20201108175458482.png)

## 4、Vue生命周期

> 什么叫生命周期：  一个事物从诞生到消亡的过程

> 钩子函数： 要让程序知道 我走到哪个声明周期了

> 有哪些生命周期函数：看官网
>
> ![image-20201108182429515](C:\Users\今天以后\AppData\Roaming\Typora\typora-user-images\image-20201108182429515.png)

![image-20201108182612141](C:\Users\今天以后\AppData\Roaming\Typora\typora-user-images\image-20201108182612141.png)