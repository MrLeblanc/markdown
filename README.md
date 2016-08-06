# jQuery添加元素


* append() - 在被选元素的结尾插入内容

* prepend() - 在被选元素的开头插入内容

* after() - 在被选元素之后插入内容

* before() - 在被选元素之前插入内容


#  jQuery获取并设置css类

* addClass() - 向被选元素添加一个或多个类

* removeClass() - 从被选元素删除一个或多个类

* toggleClass() - 对被选元素进行添加/删除类的切换操作

* css() - 设置或返回样式属性

# jQuery事件

* bind() 方法为被选元素添加一个或多个事件处理程序，并规定事件发生时运行的函数。

```js
$(document).ready(function(){
$("button").bind({
  click:function(){$("p").slideToggle();},
  mouseover:function(){$("body").css("background-color","red");},  
  mouseout:function(){$("body").css("background-color","#FFFFFF");}  
  });
});
```

* one() 方法为被选元素附加一个或多个事件处理程序，并规定当事件发生时运行的函数。
当使用 one() 方法时，每个元素只能运行一次事件处理器函数。
