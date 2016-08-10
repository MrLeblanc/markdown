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


ls -bash: ls: command not found (2012-06-25 10:09:54)
标签： it	分类： Linux学习日志

原因：在设置环境变量时，编辑profile文件没有写正确，导致在命令行下 ls等命令不能够识别。

解决方案：
 export PATH=/usr/local/sbin:/usr/local/bin:/sbin:/bin:/usr/sbin:/usr/bin:/root/bin


### npm无法启动时执行nvm use v6.3.1   


### switch语句
