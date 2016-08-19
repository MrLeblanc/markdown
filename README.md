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

  结尾default：

###  数组

```js
  var cars=new Array();
  cars[0]="Audi";
  cars[1]="BMW";
  cars[2]="Volvo";
  等同于
  var cars=new Array("Audi","BMW","Volvo");
  等同于
  var cars=["Audi","BMW","Volvo"];
```

###### 调用数组

```js
  <script>
  var person={
  firstname : "Bill",
  lastname  : "Gates",
  id        :  5566
  };
  document.write(person.lastname + "<br />");
  document.write(person["lastname"] + "<br />");
  </script>

```

### 声明新的变量的类型

```js
  var carname=new String;
  var x=      new Number;
  var y=      new Boolean;
  var cars=   new Array;
  var person= new Object;
```

### for和while

```js
  cars=["BMW","Volvo","Saab","Ford"];
  var i=0;
  for (;cars[i];)
  {
  document.write(cars[i] + "<br>");
  i++;
  }
```

```js
  cars=["BMW","Volvo","Saab","Ford"];
  var i=0;
  while (cars[i])
  {
  document.write(cars[i] + "<br>");
  i++;
  }
```

### Break 和 continue

  break 语句用于跳出循环。即break会终止后面的函数执行
  continue 用于跳过循环中的一个迭代。即continue会跳过函数中指定的一个参数但不会影响其他参数的执行

### throw

  Throw 语句
  throw 语句允许我们创建自定义错误。
  正确的技术术语是：创建或抛出异常（exception）。

```js
  <script>
    function myFunction()
    {
    try
    {
    var x=document.getElementById("demo").value;
    if(x=="")    throw "empty";
    if(isNaN(x)) throw "not a number";
    if(x>10)     throw "too high";
    if(x<5)      throw "too low";
    }
    catch(err)
    {
    var y=document.getElementById("mess");
    y.innerHTML="Error: " + err + ".";
    }
    }
  </script>
```

### document.write

绝不要使用在文档加载之后使用 document.write()。这会覆盖该文档。


### confirm(str)  弹窗判断

![confirm](http://img.mukewang.com/52e35bc60001f01a04230353.jpg)

### prompt(str1,str2)  消息对话框

![prompt](http://img.mukewang.com/52e360780001ede107090353.jpg)

### window.open([url],[窗口名称],[参数字符串])

___URL：可选参数，在窗口中要显示网页的网址或路径。如果省略这个参数，或者它的值是空字符串，那么窗口就不显示任何文档。
窗口名称：可选参数，被打开窗口的名称。
    1.该名称由字母、数字和下划线字符组成。
    2."_top"、"_blank"、"_selft"具有特殊意义的名称。
       _blank：在新窗口显示目标网页
       _self：在当前窗口显示目标网页
       _top：框架网页中在上部窗口中显示目标网页
    3.相同 name 的窗口只能创建一个，要想创建多个窗口则 name 不能相同。
    4.name 不能包含有空格。
参数字符串：可选参数，设置窗口参数，各参数用逗号隔开。___

```js
     window.open("http://www.imooc.com","_blank","width=600,height=400,menubar=yes,toolbar=yes,status=yes,scrollbars=yes,top=100,left=0")
```
### window.close()关闭窗口

### removeAttribute  删除指定方法

  a.removeAttribute("style")
  //删除a的style方法


### 变量命名规则

1. 必须以字母、下划线或美元符号开头，后面可以跟字母、下划线、美元符号和数字。

2. 变量名区分大小写，如:A与a是两个不同变量。

3. 不允许使用JavaScript关键字和保留字做变量名。

![关键字和保留字](http://img.mukewang.com/529c07c000014f5103080447.jpg)



### 100%7的含义为取余数  答案为2

### --a ++a  与  a++ a--的区别

--a ++a是以a+1或a-1为基准开始的  
a++ a--是以a为基准开始的

### for(var i in XXX){}

### 数组格式

```js
    var myarray=new Array(); //创建一个新的空数组
    myarray[0]=66; //存储第1个人的成绩
    myarray[1]=80; //存储第2个人的成绩
    myarray[2]=90; //存储第3个人的成绩
    myarray[3]=77; //存储第4个人的成绩
    myarray[4]=59; //存储第5个人的成绩


    var myarray = new Array(66,80,90,77,59);//创建数组同时赋值


    var myarray = [66,80,90,77,59];//直接输入一个数组（称 “字面量数组”）
```

    注意：数组存储的数据可以是任何类型（数字、字符、布尔值等）除了数字记得加""

### focus获取焦点 blur移除焦点

```js
  $(document).ready(function(){
    $("input").focus(function(){
      $("input").css("background-color","#FFFFCC");
    });
    $("input").blur(function(){
      $("input").css("background-color","#D6D6FF");
    });
  });
```
### javascript中onclick(this)用法介绍

```css
  <input id="myinput" type="text" value="javascript中onclick中的this" onclick="javascript:test(this);"/>
```

```js
    function test(obj){
      alert(obj); //[object HTMLInputElement]
      alert(obj.id); //myinput
      alert(obj.value); //javascript中onclick中的this
    }
```
