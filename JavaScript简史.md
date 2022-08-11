

# JavaScript

## 1.JavaScript初识

### 1.1诞生时间及作用

JavaScript诞生于<font size=5 color="blue"> 1995年</font>，它的出现主要是用于处理网页中的前端验证。所谓的前端验证，就是指检查用户输入的内容是否符合一定的规则。比如：用户名的长度，密码的长度，邮箱的格式等。



为了解决前端验证的问题，当时的浏览器巨头NetScape（网景）公司就开发出一种脚本语言，起初命名为LiveScript，后来由于SUN公司的介入更名为了JavaScript。但是你要清楚，Java和JavaScript是没有什么关系的，只不过当时Java非常流行，为了蹭热度，才将LiveScript更名为JavaScript，它们的关系就像雷锋和雷峰塔的关系一样，没啥关系。

但是，浏览器开发商不止网景一家，还有一个大家都知道的公司，微软公司，它们的主打产品是IE（Internet Explorer）浏览器，当网景公司的Netscape Navigator浏览器推出JavaScript语言时，微软就急了啊，好家伙，人网景都推出了专门用于前端验证的语言，不仅大大减少了后端程序的压力，还提高了用户的体验。我微软这么大的公司不也得整一个，在1996年，微软公司在其最新的IE3浏览器中引入了自己对JavaScript的实现JScript。

于是在市面上存在两个版本的JavaScript，一个网景公司的JavaScript和微软的JScript，虽然当时浏览器的巨头是网景，但是网景的浏览器是收费的，虽然微软的IE浏览器在全球的市场份额远远不及网景，但是微软的拳头产品是Windows操作系统，每一个操作系统都自带一个IE浏览器并且免费，那么，未来的发展大家可能也想到了，网景让微软给干倒闭了，1998年11月，网景被美国在线（AOL）收购。

老大哥就是老大哥，为了抢先获得规则制定权，网景最先将JavaScript作为草案提交给欧洲计算机制造商协会，也就是ECMA组织，希望能将JavaScript做成行业标准，最终在网景、SUN以及微软等公司的参与下，由一众程序员和相关组织人员组成的第39技术委员会也就是TC39发布了ECMA-262标准，这个标准定义了名为ECMAScript的全新脚本语言，为啥又来了个ECMAScript？

因为Java是SUN的商标，SUN授权了NetScape可以叫JavaScript，但是ECMA没有SUN的授权就不能叫JavaScript，哪怕NetScape成员特别希望ECMA把它叫做JavaScript，但是ECMA也有成员并不希望这个标准就叫JavaScript，总之经过几轮磋商和博弈，ECMAScript这个名字就定下来。

JavaScript之父      布兰登·艾奇   https://blog.csdn.net/yellowzf3/article/details/120480312



![布兰登·艾奇](assets/bf20d724447e7889148d002ee62eee7c.jpeg)
JavaScript历史发展时间表

<img src="assets/34ceed720299546a8161deab88fe16aa.png" alt="image-20201012142902870" style="zoom: 50%;" />

### 1.2 JavaScript的组成

<font size=5 color="red">ECMAScript：ECMAScript 规定了JS的编程语法和基础核心知识，是所有浏览器厂商共同遵守的一套JS语法工业标准。。</font>

“*es6是2015年6月出的。*es6全称“ECMAScript6”,是2015年6月正式发布的JavaScript语言的标准,其正式名为ECMAScript2015(ES2015),因其是ECMAScript的第6个版本,因此可简称为es6。



![image-20201012144015831](assets/584d9295990909d32b3338dbbbe9c037.png)
<font size=5 color="red">完整的JS由以下三部分组成</font>
![image-20201012144120964](assets/fafb929ac005ed0e9e2dedb433fe8eab.png)





#### 1.2.1 JavaScript的特点

<font size=5 color="red">(1)解释型语言</font>

JavaScript是一门解释型语言，所谓解释型值语言是指不需要被编译为机器码在执行，而是直接执行。由于少了编译这一步骤，所以解释型语言开发起来尤为轻松，但是解释型语言运行较慢也是它的劣势。不过解释型语言中使用了JIT技术，使得运行速度得以改善。

<font size=5 color="red">(2)动态语言</font>

JavaScript是一门动态语言，所谓的动态语言可以暂时理解为在语言中的一切内容都是不确定的。比如一个变量，这一时刻是个整型，下一时刻可能会变成字符串了。当然这个问题我们以后再谈。不过在补充一句动态语言相比静态语言性能上要差一些，不过由于JavaScript中应用的JIT技术，所以JavaScript可能是运行速度最快的动态语言了。

<font size=5 color="red">(3)基于原型的面向对象</font>

JavaScript是一门面向对象的语言。啥是对象？下次聊。

Java也是一门面向对象的语言，但是与Java不同JavaScript是基于原型的面向对象。啥是原型？下次聊。

<font size=5 color="red">(4)严格区分大小写</font>

JavaScript是严格区分大小写的，也就是abc和Abc会被解析器认为是两个不同的东西。



#### 1.2.2  概念和作用

JavaScript 是脚本语言，是一种解释性脚本语言(代码不进行预编译)
JavaScript 是一种轻量级的编程语言。
JavaScript 是可插入 HTML 页面的编程代码
JavaScript 插入 HTML 页面后，可由所有的现代浏览器执行
<font size=5 color="blue">**JavaScript 很容易入门**</font>



### 1.3 JavaScript的使用

#### 1.3.1 标签引用

==<script>JS语法 <script>==

``` javascript

<script type="text/javascript">
		 alert("Hello,World!");
</script>
```

#### 1.3.2 文件引入

在一个单独的js文件中也可以编写JavaScript代码，然后在HTML文件中使用script标签进行引用，以下是一个简单演示。

hello.js文件

```javascript
alert("Hello,World!");
// 网页弹窗弹出
console.log("Hello World!")
// 控制台弹出
```

> 	引入js文件
> 	<script src="。/hello.js" type="text/javascript"></script>



#### 1.3.3 JavaScript的输出语法

为了方便信息的输入输出，JS中提供了一些输入输出语句，其常用的语句如下：

**注意：**alert() 主要用来显示消息给用户，console.log() 用来给程序员自己看运行时的消息。



|             方法              | 说明                             | 归属   |
| :---------------------------: | -------------------------------- | ------ |
|     alert("hello,world")      | 浏览器弹出警示框                 | 浏览器 |
|        prompt("info")         | 浏览器弹出输入框，用户可以输入   | 浏览器 |
|  console.log("hello,world")   | 浏览器控制台输出一条日志（常用） | 浏览器 |
| document.write("hello,world") | 网页文档页面显示输出信息         | 网页   |

#### 1.3.4 JavaScript的注释

注释中的内容不会被解析器解析执行，但是会在源码中显示，我们一般会使用注释对程序中的内容进行解释。

JS中的注释和Java的的一致，分为两种：

- 单行注释：`// 注释内容`
- 多行注释：`/* 注释内容 */`

```javascript
<script>
    // 这是单行注释内容
    console.log("Hello,World!");

   /* 
     多行注释
    多行注释。。。
   */
</script>

```



### 1.4 JavaScript入门

#### 1.4.1  数据结构

<font color=red>JavaScript的数据结构包括：标识符、关键字、常量、变量</font>

**标识符 ** 就是指给变量、函数、属性或函数的参数起名字。

**JavaScript关键字**是指在JavaScript语言中有特定含义，成为JavaScript语法中一部分的那些字。

**常量**，顾名思义就是指不能改变的量。常量的指从定义开始就是固定的，一直到程序结束。

常量主要用于为程序提供固定和精确的值，包括数值和字符串，如数字、逻辑值真（true）、逻辑值假（false）等都是常量

**变量**，顾名思义，就是指在程序运行过程中，其值是可以改变的。

**变量命名规则**

按照下列格式规则组合起来的一或多个字符：

第一个字符必须是一个字母、下划线（ _ ）或一个美元符号（ $ ）。
其它字符可以是字母、下划线、美元符号或数字。
按照惯例，ECMAScript 标识符采用驼峰命名法。

> 1、小驼峰式命名法（lower camel case）：
> 第一个单词以小写字母开始，第二个单词的首字母大写。例如：firstName、lastName。
>
> 2、大驼峰式命名法（upper camel case）：
> 每一个单词的首字母都采用大写字母，例如：FirstName、LastName、CamelCase，也被称为 Pascal 命名法。
> 变种：StudlyCaps，是“驼峰式大小写”的变种。
>
> 补充说明，在JavaScript中：类名的[标识符](https://so.csdn.net/so/search?q=标识符&spm=1001.2101.3001.7020)一般用大驼峰式书写格式，方法和变量的标识符则多用小驼峰式书写格式。
>
> boxName、age、gender、hobby
>
> studentName、studentAge、studentGender、studentHobby

变量声明 

``` javascript

var studentName = "赵丽颖";
var age = 18;
```



**标识符变量名不能是关键字和保留字符。**
————————————————

<font size=4 color=red>关键字：</font>

![image-20201012215759481](assets/06bab955dce3d478eb0ee1880efdbf13.png)

<font size=4 color=red>保留字：</font>

![image-20201012215835171](assets/321c5fb7e148d7fa99e59440083b0a4b.png)

<font size=4 color=red>不建议使用的标识符</font>

![image-20201012215902568](assets/612f0462d3cde3f2fa410ccd8b6da15b.png)



+++



### 1.4.2  JavaScript数据类型

数据类型决定了一个数据的特征，比如：123和”123”，直观上看这两个数据都是123，但实际上前者是一个数字，而后者是一个字符串。

对于不同的数据类型我们在进行操作时会有很大的不同。

JavaScript中一共有5种基本数据类型：

#### 1、<font size=4 color=red>字符串型（String）</font>

``` js
var studentName ="赵丽颖";
var studentName2 = "Tom";
```



#### <font size=4 color=red>2 、数值型（Number）</font>

``` js
var age = 18;
/*
Number 类型用来表示整数和浮点数，最常用的功能就是用来表示10进制的整数和浮点数。
Number表示的数字大小是有限的，如果超过了这个范围，则会返回 ±Infinity。

最大值：+1.7976931348623157e+308
最小值：-1.7976931348623157e+308
0以上的最小值：5e-3248

特殊的数字：

Infinity：正无穷
-Infinity：负无穷
NaN：非法数字（Not A Number）
*/
 console.log(Number.MAX_VALUE);
        //   数字类型的最大值
 console.log(Number.MIN_VALUE);
        //数字类型的最小值
 console.log(Number.MAX_VALUE * 2) //infinity 无穷大
  console.log(-Number.MAX_VALUE * 2)//-infinity 无穷大
        // 无穷小

  //    非数字
  console.log('好好学习' - 100)  //NaN
```
<font color=red size=4>isNaN()</font>  判断非数字 并且返回一个值 如果是数字返回 false 如果不是数字返回的是true

>  console.**log**(**isNaN**(100));//是数字 返回值为false
>
>   console.**log**(**isNaN**('好好学习JS'));//不是数字 返回true

#### <font size=4 color=red>3、布尔型（Boolean）</font>

```js
var flag = true;
var cont = false;
//布尔型也被称为逻辑值类型或者真假值类型。
//布尔型只能够取真（true）和假（false）两种数值。除此以外， 其它的值都不被支持。
```



#### <font size=4 color=red>4、undefined型（Undefined）</font>

```js
var aaa;
//Undefined 类型只有一个值，即特殊的 undefined。
// 一般变量声明了但还没有定义的时候会返回 undefined，
```



#### <font size=4 color=red>5、null型（Null）</font>

```js
var totalPrice = null;
totalPrice = "238元"
// null主要用于赋值给一些可能会返回对象的变量，作为初始化。
// Null 类型是第二个只有一个值的数据类型，这个特殊的值是 null。
// undefined值实际上是由null值衍生出来的，所以如果比较undefined和null是否相等，会返回true。
// 从语义上看null表示的是一个空的对象，所以使用typeof检查null会返回一个Object。
```

<font size="4" >undefined 代表的含义是**未定义**，null 代表的含义是**空对象**。</font>

这5种之外的类型都称为**Object（对象）**

<font size=4 color=red>Object（对象）</font>

```js
var array = ['赵丽颖','23',true];
var obj = {};
```

所以总的来看JavaScript中共有六种数据类型

### 1.4.3 JavaScript运算符

#### **1. typeof运算符**

可以来获得一个值的类型

它会将该值的类型以字符串的形式返回（number 、string、 boolean 、undefined、 object）

```js
// typeof 数据  判断数值的类型
typeof 100;// number
typeof 'zhaoliying' ;//string
```

#### **2.算数运算符**

算术运算符用于表达式计算。

```javascript
var a = 10;
a + 15
console.log(a+15)

```

<font size=4 color=red>假设y= 5，下面的表格解释了这些运算符</font>

| 运算符 |      描述      |      举例运算      | x运算结果  | y运算结果  |
| :----: | :------------: | :----------------: | :--------: | :--------: |
|   +    |      加法      |       x=y+2        |     7      |     5      |
|   -    |      减法      |       x=y-2        |     3      |     5      |
|   *    |      乘法      |       x=y*2        |     10     |     5      |
|   /    |      除法      |       x=y/2        |    2.5     |     5      |
|   %    | 取模（求余数） |       x=y%2        |     1      |     5      |
|   ++   |     自增+1     | 【x=++y】【x=y++】 | 【6】【6】 | 【6】【5】 |
|  （）  |  提高计算顺序  |     x=10*(y+2)     |     72     |     5      |

#### **3.赋值运算符**

<font size=4 color=red>假设x= 10，y等于5 ，下面的表格解释了这些运算符</font>

| 运算符 | 举例 | 等同于 | x运算结果 |
| :----: | :--: | :----: | :-------: |
|   =    | x=y  |        |    x=5    |
|   +=   | x+=y | x=x+y  |   x=15    |
|   -=   | x-=y | x=x-y  |    x=5    |
|   *=   | x*=y | x=x*y  |   x=50    |
|   /=   | x/=y | x=x/y  |    x=2    |
|   %=   | x%=y | x=x%y  |    x=0    |

#### **4.逻辑运算符**

<font size=4 color=red>假设x= 10，y等于5 ，下面的表格解释了这些运算符</font>

| 运算符 | 描述                                            | 举例                           |
| ------ | ----------------------------------------------- | ------------------------------ |
| &&     | and 与（两边都为true，结果为true，否则为false） | （x>5）&&(y<1) 结果为  false   |
| \|\|   | or 或 （一边为true，结果为真，否则为假）        | （x>5）\|\| (y<1) 结果为  true |
| ！     | not 取反                                        | （x==y）结果为true             |

关于逻辑运算

+ && 与：&&可以对符号两侧的值进行与运算并返回结果，运算规则如下：
  两个值中只要有一个值为false，就返回false，只有两个值都为true时，才会返回true

  <font color=red size=>JS中的“与”属于短路的与，如果第一个值为false，则不会检查第二个值
  非布尔值时：如果两个都为true，则返回第二个值，如果两个值中有false，则返回靠前的false的值</font>

+ || 或：||可以对符号两侧的值进行或运算并返回结果，运算规则如下：
  两个值中只要有一个true，就返回true，只有两个值都为false，才会返回false

  
  
  <font color=red>JS中的“或”属于短路的或，如果第一个值为true，则不会检查第二个值
  非布尔值时：如果两个都为false ，则返回第二个值，如果两个值中有true，则返回靠前的true的值</font>
  
+ ! 非：!可以用来对一个值进行非运算，所谓非运算就是对一个布尔值进行取反操作，true变false，false变true，运算规则如下：
  如果对一个值进行两次取反，它不会变化
  
+ <font  color=red>非布尔值时：先会将其转换为布尔值，然后再取反，所以我们可以利用该特点，来将一个其它的数据类型转换为布尔值，可以为一个任意数据类型取两次反，来将其转换为布尔值，原理和Boolean()函数一样</font>



#### **5.比较运算符**

比较运算符
比较运算符用来比较两个值是否相等，如果相等会返回true，否则返回false。

``` js

// 比较运算符用来比较两个值是否相等，如果相等会返回true，否则返回false。

// 使用 == 来做相等运算
  
// 当使用==来比较两个值时，如果值的类型不同，则会自动进行类型转换，将其转换为相同的类型，然后在比较
// 使用 != 来做不相等运算
// 不相等用来判断两个值是否不相等，如果不相等返回true，否则返回false，不相等也会对变量进行自动的类型转换，如果转换后相等它也会返回false
// 使用 === 来做全等运算
// 用来判断两个值是否全等，它和相等类似，不同的是它不会做自动的类型转换，如果两个值的类型不同，直接返回false
// 使用 !== 来做不全等运算
// 用来判断两个值是否不全等，它和不等类似，不同的是它不会做自动的类型转换，如果两个值的类型不同，直接返回true

```



#### **6.条件运算符**

**条件运算符是唯一的三目运算符，其语法格式如下：**

**三目运算**

~~~js

~~~



``` javascript

b ? x : y
/* b 操作数必须是一个布尔型的表达式，x 和 y 是任意类型的值。

如果操作数 b 的返回值为 true，则执行 x 操作数，并返回该表达式的值。
如果操作数 b 的返回值为 false，则执行 y 操作数，并返回该表达式的值。*/
```

**7.运算层级**

 1.单目运算符

```javascript
/* 
单目运算符是指运算所需变量为一个的运算符，又叫一元运算符，其中有逻辑非运算符：!、按位取反运算符：~、自增自减运算符：++， –等。
逻辑非运算符【!】自增自减运算符【++， –】、负号运算符【-】
*/

```

2. 双目运算符

   ``` javascript
   双目运算符就是对两个变量进行操作
   初等运算符　下标运算符【[]】、分量运算符的指向结构体成员运算符【->】、结构体成员运算符【.】
   算术运算符
   乘法运算符【*】、除法运算符【/】、取余运算符【%】 、加法运算符【+】、减法运算符【-】
   
   关系运算符
   
   等于运算符【==】、不等于运算符【!=】 、关系运算符【< > <= >= 】
   逻辑与运算符【&&】 、逻辑或运算符【||】、逻辑非运算符【！】
   
   赋值运算符
   赋值运算符【= += -= *= /= %= >>= <<= &= |= ^=】
   逗号运算符
   逗号运算符【,】
   
   
   ```

   ### *7.条件运算符*

``` javascript
// 逗号，运算符

var a = 1,b = 2,c = 3,d = 4;
//等价于
var a = 1;
var b = 2;
var c = 3;
var d = 4;
```

####    7.强制类型转化

强制类型转换指将一个数据类型强制转换为其它的数据类型。一般是指，将其它的数据类型转换为String、Number、Boolean。

##### 1.转换为String类型

将其它数值转换为字符串有三种方式：toString()、String()、 拼串。

方式一：调用被转换数据类型的toString()方法，该方法不会影响到原变量，它会将转换的结果返回，但是注意：null和undefined这两个值没有toString()方法，如果调用它们的方法，会报错
``` js
var a = 123;
a = a.toString();
console.log(a);
console.log(typeof a);

```

方法二：

``` js
/*调用String()函数，并将被转换的数据作为参数传递给函数，使用String()函数做强制类型转换时，对于Number和Boolean实际上就是调用的toString()方法，但是对于null和undefined，就不会调用toString()方法，它会将 null 直接转换为 “null”，将 undefined 直接转换为 “undefined”。*/

var a = 123;
a = String(a);
console.log(a);
console.log(typeof a);

var b = undefined;
b = String(b);
console.log(b);
console.log(typeof b);

var c = null;
c = String(c);
console.log(c);
console.log(typeof c);

```

方法三

``` js
var a = 123;
a = a + "";
console.log(a);
console.log(typeof a);
```



##### 2.转换为Number类型

~~~js
/*
有三个函数可以把非数值转换为数值：Number()、parseInt() 和parseFloat()。Number()可以用来转换任意类型的数据，而后两者只能用于转换字符串。parseInt()只会将字符串转换为整数，而parseFloat()可以将字符串转换为浮点数。

方式一：使用Number()函数

字符串 --> 数字
如果是纯数字的字符串，则直接将其转换为数字
如果字符串中有非数字的内容，则转换为NaN
如果字符串是一个空串或者是一个全是空格的字符串，则转换为0
布尔 --> 数字
true 转成 1
false 转成 0
null --> 数字
null 转成 0
undefined --> 数字
undefined 转成 NaN


*/
// parseInt() 把一个字符串转换为一个整数
var a = "123";
a = parseInt(a);
console.log(a);
console.log(typeof a);
// parseFloat() 把一个字符串转换为一个浮点数
var a = "123.456";
a = parseFloat(a);
console.log(a);
console.log(typeof a);
//如果对非String使用parseInt()或parseFloat()，它会先将其转换为String然后在操作
~~~



##### **3、转换为Boolean类型**

~~~js
/*将其它的数据类型转换为Boolean，只能使用Boolean()函数。

使用Boolean()函数
数字 —> 布尔
除了0和NaN，其余的都是true
字符串 —> 布尔
除了空串，其余的都是true
null和undefined都会转换为false
对象也会转换为true*/
~~~



## 2.JavaScript 初级

### **1、条件语句**

#### 1、  if语句

第一种形式

``` javascript
if(条件表达式){
    执行语句
}
  
var age = 16;
if (age < 18) {
    console.log("未成年");
}


```

1.2 第二种形式

``` javascript
var age = 16;
if (age < 18) {
    // 条件成立执行语句
    console.log("未成年");
} else {
    // 条件不成立 执行语句
    console.log("已成年");
}

```

1.3 第三种形式

``` javascript
var age = 18;
if (age < 18) {
    console.log("小于18岁了");
} else if (age == 18) {
    console.log("已经18岁了");
}  else if(age == 10)  
      console.log('已经是十岁了')
else {
    console.log("大于18岁了")
}
// else if () 理论上可以无限次
```



#### **2 、switch…case 语句**

switch…case是另一种流程控制语句。

switch语句更适用于多条分支使用同一条语句的情况。

break：break主要用在循环语句或者switch语句中，用来退出整个语句块。

``` javascript
/*switch (语句) {
    case 表达式1:
        语句...
    case 表达式2:
        语句...
    default:
        语句...
}*/

var today = 1;
switch (today) {
    case 1:
        console.log("星期一");
        break;
    case 2:
        console.log("星期二");
        break;
    case 3:
        console.log("星期三");
        break;
    case 4:
        console.log("星期四");
        break;
    case 5:
        console.log("星期五");
        break;
    case 6:
        console.log("星期六");
        break;
    case 7:
        console.log("星期日");
        break;
    default:
        // 以上分支都不匹配时时执行
        console.log("输入错误");
}

```



### 2、循环语句

#### 1、while循环

while语句是一个最基本的循环语句，while语句也被称为while循环。

``` js
while(条件表达式){
    循环体语句...
}
    
var i = 1;
while (i <= 10) {
    console.log(i);
    i++;
}

```



#### **2、do...while循环**

do…while和while非常类似，只不过它会在循环的尾部而不是顶部检查表达式的值

因此，do…while循环会至少执行一次。

相比于while，do…while的使用情况并不 是很多。

``` js
    var i = 1;
    do {
       console.log(i);
    } while (i >= 3)

```

#### 3、for循环

for语句也是循环控制语句，我们也称它为for循环。大部分循环都会有一个计数器用以控制循环执行的次数， 计数器的三个关键操作是

初始化、检测和更新。for语句 就将这三步操作明确为了语法的一部分。

```js
for(初始化表达式 ; 条件表达式 ; 更新表达式){
    语句...
}

 for (var i = 1; i <= 10; i++) {
    console.log(i);
}
```

**3.2 双重for循环**

```js
 for (var i = 1; i <= 10; i++) {
    for(var j = 1; j<= 3;j++){
         console.log('好好学习');
    }
}
```

``` js
    for(var i=0;i<3;i++){
       
            if(i==1){
                break;
            }
            console.log('好好学习')
        }
    // 显示次数 为1

```




> break用于完全结束一个循环，跳出循环体。不管是哪种循环，一旦在循环体中遇到break，系统将完全结束循环，开始执行循环之后的代码。 **break只能跳出其所在的循环，如果是嵌套循环，需要按照嵌套的层次，逐步使用break来跳出. 。**
>
> 

``` js
      for (var i = 0; i < 3; i++) {

            if (i == 1) {
                continue;
            }
            console.log('好好学习')
        }



```

> continue的功能和break有点类似，区别是**continue只是中止本次循环，接着开始下一次循环**







###3.  JS常用对象和方法

#### 1.文档写入

```    javascript
document.open()
document.write("<p>Hello world!</p>");
// 在网页中写入一个标签
dcument.write("<p>I am a fish</p>");
document.write("<p>The number is 42</p>");
document.close();
```

#### 2.字符串连接

1.<font size="4" color=red>普通字符串拼接  使用 + 号</font>  字符串 使用  **'单引号 '** 或者  **“ 双引号 ”** 包裹起来的数据

``` javascript
var stuName = '刘德华'
var age = 60;
var result = stuName + "今年"+ age +"岁了";
console.log(result) //刘德华今年60岁了

// 字符串型数据 + 任何数据类型的值结果都是字符串
```

<font size="4" color=red>2、ES6新增模板字符串</font> 

``` js
 // 1.什么是模板字符串？

 // 模板字符串：是允许嵌入表达式的字符串，
//（可以使用多行字符串和字符串[插值]功能）
//它与一般字符串不同，会保留空格，换行符和缩进

 // 2.用法 使用反撇号 
 ` hello 
   你好
      word
      世界
 `
 
 
```



  3.使用字符串插值 功能



```js
var a = "蜜";
var b = "探";
var text = `秘密的${a}, 探案的${b}`;
console.log(text);		// 秘密的蜜, 探案的探

```









4. for循环案例

    打印九九乘法表

``` javascript
  document.write("<table>");
        for (let i = 1; i <= 9; i++) {
            document.write("<tr>");
            for (let j = 1; j <= i; j++) {
                document.write("<td>");
                document.write(j + "*" + i + "=" + i * j);
                document.write("</td>");
            }
            document.write("</tr>");
        }
        document.write("</table>");
        document.write("<hr>");
        
        // 2. 第二方法，要求：不创建表去实现。
        for (let i = 1; i <= 9; i++) {
            for (let j = 1; j <= i; j++) {
                // document.write(j + "*" + i + "=" + i * j);
                // ${变量名称}， ${}占位符
                document.write(`${j}*${i}=${i * j}`);
                document.write(`&nbsp;&nbsp;&nbsp;&nbsp;`);
            }
            document.write("<br>");
        }
```



#### 3. Js转义符

无法被键盘录入的字符、被当作特殊用途而需要转换回它原来的意义的字符。而转义字符的转义是指字符已经被转换了意义。

![image-20220717164832885](assets/image-20220717164832885.png)

```js

<Script Language="JAVAScript">

    //用(\")表示(")
    document.write("我们的\"爱人\"");
    document.write("<hr>");
    //用(\\)表示(\)
    document.write("文件在C:\\Windows\\下");
    document.write("<hr>");
    //用(\n)表示换行
    alert("好好学习\n天天向上");
    document.write("<hr>");
    //用(\n)表示换行
    document.write("<pre>是MM就\n亲一下</pre>");
    document.write("<hr>");
</Script>
```



> 说明:
>
> 1、"\n"这个转义字符则常与alert()搭配使用，效果相当于在文本编辑器当中按下“Enter”键(VBScript里是常量"vbCrLf")。
>
> 2、如果一定要在document.write()当中使用"\n",必须搭配HTML的<PRE>标记才有作用。（一般用<br>）。



### 4.数学对象 Math

```javascript
/*固定值*/
console.log("PI = " + Math.PI); // 圆周率
console.log("E  = " + Math.E);  // 返回算术常量 e，即自然对数的底数（约等于2.718）。
console.log("E2 = " + Math.LN2); //LN2	返回 2 的自然对数（约等于0.693）。
console.log("SQR2 = " + Math.SQRT2);返回 2 的平方根（约等于 1.414）。
console.log("===============");
/*正数*/
console.log(Math.abs(1));        //可以用来计算一个数的绝对值
console.log(Math.ceil(1.1));     //可以对一个数进行向上取整，小数位只有有值就自动进1
console.log(Math.floor(1.99));   //可以对一个数进行向下取整，小数部分会被舍掉
console.log(Math.round(1.4));    //可以对一个数进行四舍五入取整
console.log("===============");
/*负数*/
console.log(Math.abs(-1));       //可以用来计算一个数的绝对值
console.log(Math.ceil(-1.1));    //可以对一个数进行向上取整，小数部分会被舍掉
console.log(Math.floor(-1.99));  //可以对一个数进行向下取整，小数位只有有值就自动进1
console.log(Math.round(-1.4));   //可以对一个数进行四舍五入取整
console.log("===============");

console.log("===============");
/*数学运算*/
console.log(Math.pow(12, 3));   //Math.pow(x,y)：返回x的y次幂
console.log(Math.sqrt(4));      //Math.sqrt(x) ：返回x的平方根

/*随机数*/
//Math.random()：可以用来生成一个0-1之间的随机数
console.log(Math.round(Math.random() * 10));            //生成一个0-10之间的随机数
console.log(Math.round(Math.random() * (10 - 1) + 1));  //生成一个1-10之间的随机数
//生成一个0-x之间的随机数：Math.round(Math.random()*x)
//生成一个x-y之间的随机数：Math.round(Math.random()*(y-x)+x)


console.log(parseInt("12.5rem"));// 12
console.log(parseInt("3.1415926"));// 12

parseInt 和 parseFloat 的作用。
它们可以从字符串中“读取”数字，直到无法读取为止。如果发生 error，则返回收集到的数字。
函数 parseInt 返回一个整数，
parseFloat 返回一个浮点数
*/：
 // toFixed(x) x表示小数的个数
  var result = Math.PI;
  console.log(result.toFixed(2));//3.14
/*
  console.log(parseInt('a123'));
// 当没有数字可读时会发生这种情况： parseInt/parseFloat 会返回 NaN。
```



### 5.日期对象 Date

##### 1.Date方法的使用

如果括号里面有时间，就返回参数里面的时间。例如日期格式字符串为 `‘2019-5-1’`，可以写成`new Date('2019-5-1')` 或者 `new Date('2019/5/1')`

- 如果Date()不写参数，就返回当前时间
- 如果Date(0)写参数0，就返回1970年1月1日 0点
- 如果Date()里面写参数，就返回括号里面输入的时间

``` js
var date = new Date();
console.log(date);
// 获取当前时间 必须实例化 

// 1.如果没有参数，返回当前系统的当前时间
var now = new Date();
console.log(now);


// 2.参数常用的写法 数字型 2019,10,1  字符串型 '2019-10-1 8:8:8' 时分秒
// 如果Date()里面写参数，就返回括号里面输入的时间 
var data = new Date(2019,10,1);
console.log(data);  // 返回的是11月不是10月

var data2 = new Date('2019-10-1 8:8:8');
console.log(data2);

```



##### 2.获取当前时间

``` js


console.log(date.getFullYear());//获取当前日期对象的年份(四位数字年份)
console.log(date.getMonth());//获取当前日期对象的月份(0 ~ 11)
console.log(date.getDate());//获取当前日期对象的日数(1 ~ 31)
console.log(date.getHours());//获取当前日期对象的小时(0 ~ 23)
console.log(date.getMinutes());//获取当前日期对象的分钟(0 ~ 59)
console.log(date.getSeconds());//获取当前日期对象的秒钟(0 ~ 59)
console.log(date.getTime());//获取当前时间到1970年1月1日午夜的毫秒数
console.log(date.getMilliseconds());//获取当前日期对象的毫秒(0 ~ 999)

```



##### 3.时间戳 获取总的毫秒数

- `date.valueOf()` ：得到现在时间距离1970.1.1总的毫秒数
- `date.getTime()` ：得到现在时间距离1970.1.1总的毫秒数

``` js
// 获取Date总的毫秒数 不是当前时间的毫秒数 而是距离1970年1月1号过了多少毫秒数

// 实例化Date对象
var date = new Date();

// 1 .通过 valueOf()  getTime() 用于获取对象的原始值
console.log(date.valueOf());  //得到现在时间距离1970.1.1总的毫秒数
console.log(date.getTime());

// 2.简单的写法
var date1 = +new Date();  // +new Date()返回的就是从1970年1月1日0点到现在的总毫秒数，
console.log(date1);



/*年
var 差值=将来-现在

差值/1000---->秒
差值/1000/60------>分钟
差值/1000/60/60------>小时
差值/1000/60/60/24------>天
差值/1000/60/60/24/30------>月
*/

```

##### 3.京东秒杀倒计时

``` js


    var nowTime = new Date(); //没有参数，返回的是当前时间总的毫秒数
    var inputTime = new Date('2020-11-09 18:29:00'); // 有参数，返回的是用户输入时间的总毫秒数
    var times = (inputTime - nowTime) / 1000; //times就是剩余时间的总的秒数

    var d = parseInt(times / 60 / 60 / 24); //天数
    d < 10 ? '0' + d : d;
    var h = parseInt(times / 60 / 60 % 24); //小时
    h < 10 ? '0' + h : h;
    var m = parseInt(times / 60 % 60); //分
    m < 10 ? '0' + m : m;
    var s = parseInt(times % 60); //秒
    s < 10 ? '0' + s : s;
    var shijian =  d + '天' + h + '时' + m + '分' + s + '秒';



```



+++

### 5.数组对象

##### 1.数组概述

数组是一种用于表达有顺序关系的值的集合，也就是数据元素的有序集合。

JavaScript中是支持数组可以是不同的元素，数组内的各个值被称作元素，每一个元素都可以通过索引（下标）来快速读取，索引是从零开始的整数

##### 2.数组的创建和使用



~~~ js
// 1.使用new对象创建
var arr = new Array();
arr[0] = 1;
arr[1] = 2;
arr[2] = 3;
arr[3] = 4;
arr[4] = 5;
// 2.使用字面量创建
var arr = [];//声明一个空数组
var arr = [1, 2, 3, 4, 5, 6, 7, 8, 9];

// 3.遍历数组
for (var i = 0; i < arr.length; i++) {
    console.log(arr[i]);
}

~~~

##### 3.数组属性和API方法

###### **1.length()属性 **

**设置或返回数组元素的个数**

~~~	js
var arr = [1,2,3,4];
console.log(arr.length);

~~~

###### **2. constructor**

**属性：返回创建数组对象的原型函数**

~~~ js
var arr = [1,2,3,4];
console.log(arr.constructor);
~~~

###### **3.push()**

**方法：可以向数组的末尾添加一个或多个元素，并返回数组的新的长度**

```js
var arr = ["孙悟空", "猪八戒", "沙和尚"];
var result = arr.push("唐僧", "蜘蛛精", "白骨精", "玉兔精");
console.log(arr); // 新数组
console.log(result); // 7

```

###### **4. pop()**

**方法：该方法可以删除数组的最后一个元素，并将被删除的元素作为返回值返回**

~~~ js
var arr = ["孙悟空", "猪八戒", "沙和尚"];
var result = arr.pop();
console.log(arr);
console.log(result);

~~~

###### **5.unshift()**

**方法演示：该方法向数组开头添加一个或多个元素，并返回新的数组长度**

~~~js
var arr = ["孙悟空", "猪八戒", "沙和尚"];
var result = arr.unshift("牛魔王", "二郎神");
console.log(arr);
console.log(result);

~~~

###### **6.shift()**

**方法演示：该方法可以删除数组的第一个元素，并将被删除的元素作为返回值返**

~~~js
var arr = ["孙悟空", "猪八戒", "沙和尚"];
var result = arr.shift();
console.log(arr);
console.log(result);

~~~



###### **7.slice()**

**方法：用来从数组提取指定元素，该方法不会改变元素数组，而是将截取到的元素封装到一个新数组中返回**

- 第一个参数：截取开始的位置的索引，包含开始索引
- 第二个参数：截取结束的位置的索引，不包含结束索引，第二个参数可以省略不写，此时会截取从开始索引往后的所有元素
- <font color=red size=4>注意</font>：索引可以传递一个负值，如果传递一个负值，则从后往前计算，-1代表倒数第一个，-2代表倒数第二个。

~~~js
var arr = ["孙悟空", "猪八戒", "沙和尚", "唐僧", "白骨精"];
var result = arr.slice(1, 4);
console.log(result);
result = arr.slice(3);
console.log(result);
result = arr.slice(1, -2);
console.log(result);

~~~



###### **8.splice()**

**方法：用于删除数组中的指定元素，该方法会影响到原数组，会将指定元素从原数组中删除，并将被删除的元素作为返回值返回**

- 第一个参数：表示开始位置的索引
- 第二个参数：表示要删除的元素数量
- 第三个参数及以后参数：可以传递一些新的元素，这些元素将会自动插入到开始位置索引前边

~~~ js
var arr = ["孙悟空", "猪八戒", "沙和尚", "唐僧", "白骨精"];
var result = arr.splice(3, 2);
console.log(arr);
console.log(result);
result = arr.splice(1, 0, "牛魔王", "铁扇公主", "红孩儿");
console.log(arr);
console.log(result);

~~~



###### **9.concat()**

**方法：该方法可以连接两个或多个数组，并将新的数组返回，该方法不会对原数组产生影响**

~~~js
var arr = ["孙悟空", "猪八戒", "沙和尚"];
var arr2 = ["白骨精", "玉兔精", "蜘蛛精"];
var arr3 = ["二郎神", "太上老君", "玉皇大帝"];
var result = arr.concat(arr2, arr3, "牛魔王", "铁扇公主");
console.log(result);
~~~



###### **10.join()**

**方法：可以将数组转换为一个字符串，该方法不会对原数组产生影响，而是将转换后的字符串作为结果返回，**

**在join()中可以指定一个字符串作为参数，这个字符串将会成为数组中元素的连接符，如果不指定连接符，则默认使用，作为连接符**

~~~ js
var arr = ["孙悟空", "猪八戒", "沙和尚"];
var result = arr.join("@-@");
console.log(result);

~~~



###### **11.reverse()**

**方法：该方法用来反转数组（前边的去后边，后边的去前边），该方法会直接修改原数组**

~~~js
var arr = ["孙悟空", "猪八戒", "沙和尚"];
arr.reverse();
console.log(arr);

~~~



###### **12.sort()**

**方法：该方法可以用来对数组中的元素进行排序，也会影响原数组，默认会按照Unicode编码进行排序**

~~~js
var arr = ["b", "c", "a"];
arr.sort();
console.log(arr);

/* 可以在sort()添加一个回调函数，来指定排序规则，回调函数中需要定义两个形参，浏览器将会分别使用数组中的元素作为实参去调用回调函数，使用哪个元素调用不确定，但是肯定的是在数组中a一定在b前边，浏览器会根据回调函数的返回值来决定元素的顺序，如下：

如果返回一个大于0的值，则元素会交换位置
如果返回一个小于0的值，则元素位置不变
如果返回一个等于0的值，则认为两个元素相等，也不交换位置 */
var arr = [1, 3, 2, 11, 5, 6];
arr.sort(function (a, b) {
    return a - b;
});
console.log(arr);

~~~



###### **13.forEach() 遍历数组**

forEach()方法需要一个函数作为参数，像这种函数，由我们创建但是不由我们调用的，我们称为回调函数。数组中有几个元素函数就会执行几次，每次执行时，浏览器会将遍历到的元素，以实参的形式传递进来，我们可以来定义形参，来读取这些内容，浏览器会在回调函数中传递三个参数：

第一个参数：就是当前正在遍历的元素
第二个参数：就是当前正在遍历的元素的索引
第三个参数：就是正在遍历的数组
注意：这个方法只支持IE8以上的浏览器，IE8及以下的浏览器均不支持

~~~
var arr = ["孙悟空", "猪八戒", "沙和尚"];
arr.forEach(function (value, index, obj) {
    console.log(value + " #### " + index + " #### " + obj);
});

~~~

###### **16.Array.isArray()**

判断一个变量是否为数组，是返回true，否则返回false

```js
var arr = [1,2,3];
console.log(Array.isArray(arr));// true

```

##### 4.数组高级方法

###### 1.sort() 方法

对数组的元素进行排序,改变原有数组。

~~~js
sort() 该方法用于对数组元素进行排序 ，默认按照字母升序，当然也可以排列数字
        // var arr = ["o","z","c","m","f","h","a"];
        // console.log(arr.sort());//c f h m o
        var arr = [4, 8, 5, 7, 10];
        function reorder(a, b) {
            // 如果return返回-1(或者小于0的值),表示a小于b,数组排序中a会排在b之前
            // 如果return返回1（大于0的值）,表示a大于b,数组排序中a会排在b之后
            // 如果return返回0,表示a与b相等,其位置保持不变

            // return a - b;
            //  数字升序（从小到大）

            // return b - a;
            // 数字降序（从大到小）
        };
        // 数组从大到小排列
        console.log(arr.sort(reorder));
~~~



######  2.map()方法

遍历数组，对数组中的每一项进行操作后，并且返回一个新数组，不会修改原来的数组

~~~js
  var student = ["小明", "小红", "小刚", "小亮"];// ["三号学生小明","三号学生小红","三号学生小刚",]
        var newStuent = student.map(function (item) {
            // item 是数组中的每一个元素

            // console.log("三好学生" + item);
            return "三好学生" + item

        })
        // console.log(student)
        // console.log(newStuent);
~~~



###### 3. filter方法

 该方法把数组中的某些元素过滤删除掉，然后返回剩下的元素,不会影响原数组

~~~js

        var arrnum = [4, 8, 5, 7, 10, 1, 3];// 过滤掉偶数，返回奇数
        var oddArr = arrnum.filter(function (value, index, arr) {
            // console.log(x);
            //根据返回值是true还是false决定是否保留该元素
            return value % 2 !== 0;
            // console.log(value,index,arr);
        })
        // console.log(oddArr);//[5,7,1,3]
        // console.log(arr);

        // 利用filter方法 ，可以轻松的去掉重复元素(去重)
        var food = ["米饭", "馒头", "面条", "米饭", "馒头", "水果"];//
        var newFood = food.filter(function (value, index, food) {
            return food.indexOf(value) === index;
            // 米饭  1   ==      4
        });
        // console.log(newFood);
~~~



###### 4.fill方法

​    使用特定值填充数组中一个或者多个元素，

​    // 当只有一个值时，该方法会用参数中的值填满整个数组

~~~js
 var arr = [1, 2, 3, 4, "aa", "cc", 5];
        // arr.fill(100);
        // console.log(arr);
        // 如果你不想改变数组中的所有值，只改变其中一部分
        // array.fill(value, start, end);
		// value 填充的值  start是开始位置 ，end是结束位置（不包括结束位置，如果不写，默认替换到结尾）
        // arr.fill("Array", 4, 6);
        // console.log(arr);

~~~



###### 5.every() / some();

```js
// 判断数组中每一项的元素值是否满足条件，只有所有项都满足，才会返回ture,不会改变原数组
    var arr = [1, 2, 3, 4, 5, "i"]
    var newarr = arr.**every**(function (value) {
      return value < 10;
    })

// some() //可以理解为或元素，判断数组中只要有一项满足条件，就返回true，否则为false
     var arr = [1, 2, 3, 4, 5, 100, 200]
        var newarr = arr.some(function (value) {
            return value > 10;
        })
```



###### 6 includes()

~~~js
  // 8. includes() 判断数组中是否包含某一个元素，如果包含返回true，否则false
        // 指定查找位置(元素，开始位置)
        var arr = [1, 100, 2, 3, 4, 5, 200];
        var mx = arr.includes(100);// true
        var mx2 = arr.includes(100, 3);//false
        console.log(mx);
        console.log(mx2);
~~~



###### 7.reduce() / reduceRight()

两个方法 都会实现迭代数组中的所有元素（即累加器），然后把计算结果返回

~~~js
        // reduce()方法从数组第一项开始，逐个遍历到最后
        // reduceRight() 方法 从数组最后一项开始，逐个遍历到第一项
        var arr = [1, 2, 3, 4, 5, 100, 200];// 315
        var sum = arr.reduceRight(function (prev, cur, index, array) {
            // prev 前一个值 ,cur当前值 ,index索引号，array数组
            // console.log(cur);
            // console.log(index);
            return prev + cur
        })
        console.log(sum);//315
~~~



###### 8.find() 和 findIndex()

~~~js

    // 回调函数 可以接收三个参数，数组中的某个元素，元素对应的索引位置，以及该数组
    // 该回调函数给指定的元素满足定义条件时返回true，
    // 这两个方法都会在回调函数第一次返回true时停止查找
    // 2和3的公倍数
    var arr = [36, 42, 77, 12, 6];

    // 第一个满足条件的元素值
    var result = arr.find(function (value, index, array) {
    // console.log(this)
    return value % 6 !== 0;
    })
    console.log(result);// 77

    // 返回满足条件元素的索引位置
    var result = arr.findIndex(function (value, index, array) {
     return value % 6 !== 0;
    })
    console.log(result);// 2
    arr.splice(result, 1);
    console.log(arr);
~~~





### 6.字符串方法



##### **1.constructor属性：**

**返回创建字符串对象的原型函数**

```js
var str = "Hello,World!";
console.dir(str.constructor);

```



##### **2.length属性：**

**可以用来获取字符串的长度**

~~~js
var str = "Hello,World!";
console.log(str.length);

~~~

##### **2.charAt**(index)

**返回指定索引所在的字符 默认第一个字符位置索引为0**

~~~js
var str = "Hello,World!";
console.log(str.charAt(4)); // o
~~~



##### **3.charCodeAt()：**

**该方法获取指定位置字符的字符编码（Unicode编码 / ASCII码值）**

~~~js
var str = "Hello,World!";
console.log(str.charCodeAt(1));

~~~



##### **4.concat()：**

**该方法可以用来连接两个或多个字符串**

~~~ js
var str = "Hello,World!";
console.log(str.concat("你好，", "世界！"));

~~~



##### **5.indexof()：**

**该方法可以检索一个字符串中是否含有指定内容，如果字符串中含有该内容，则会返回其第一次出现的索引，如果没有找到指定的内容，则返回-1，可以指定一个第二个参数，指定开始查找的位置**

~~~js
var str = "Hello,World!";
console.log(str.indexOf("o"));
console.log(str.indexOf("o", 5));

// lastIndexOf()方法 倒排序
~~~



##### **7. slice()方法：**

**可以从字符串中截取指定的内容，不会影响原字符串，而是将截取到内容返回**

参数：

- 第一个参数：开始位置的索引（包括开始位置）
- 第二个参数：结束位置的索引（不包括结束位置），如果省略第二个参数，则会截取到后边所有的
- 注意：也可以传递一个负数作为参数，负数的话将会从后边计算

~~~js
var str = "Hello,World!";
var result = str.slice(1, 4);
console.log(result);
result = str.slice(1);
console.log(result);
result = str.slice(1, -1);
console.log(result);

~~~



##### **8.substring()：**

**可以用来截取一个字符串，它和slice()类似**

参数：

- 第一个参数：开始截取位置的索引（包括开始位置）
- 第二个参数：结束位置的索引（不包括结束位置），如果省略第二个参数，则会截取到后边所有的



##### **9.substr()：**

**该方法用来截取字符串**

- 第一个参数：截取开始位置的索引
- 第二个参数：截取的长度

~~~js
var str = "Hello,World!";
var result = str.substr(6, 6);
console.log(result);

~~~



##### **10.split()方法：**

**该方法可以将一个字符串拆分为一个数组，需要一个字符串作为参数，将会根据该字符串去拆分数组**

~~~js
var str = "Hello,World!";
var result = str.split(",");
console.log(result);
~~~



##### **11.toUpperCase()：**

**将一个字符串转换为大写并返回**

~~~js
var str = "Hello,World!";
var result = str.toUpperCase();
console.log(result);

~~~



##### **12.toLowerCase()：**

**将一个字符串转换为小写并返回**

~~~js
var str = "Hello,World!";
var result = str.toLowerCase();
console.log(result);

~~~



##### 13.str.startsWith()

**该方法确定字符串是否以指定字符串的字符开头，返回true和false 两种值**

```js
 result = "Hello,World你好世界赵丽颖";      
console.log(result.startsWith("天"));// flase

```



#####  14.str.endsWith（）

 **该方法确定字符串是否以指定字符串的字符结尾**，返回true和false 两种值

~~~js
 result = "Hello,World你好世界赵丽颖";
 console.log(result.endsWith("颖")); //true
~~~

**15.trim()**

**该方法删除字符串前后空格**

~~~js

        var str = "   中国万岁        ";
        console.log(str.length);// 15
        var newstr = str.trim();
        console.log(newstr);//"中国万岁"
        console.log(newstr.length);//4
        // 16.str.trimEnd（）== trimRight()是此方法的别名 从字符串末尾删除空格。

        // 17. str.trimStart() == trimLeft()是此方法的别名  从字符串开头删除空格
~~~

#####    16. str1.includes(str2) 。

**判断字符串1中是否包含另一个字符串2，返回true或者false**

    var sentence = '中国万岁';
    var word = '中国';
    console.log(sentence.includes(word));//  true

##### 17.replace()

~~~js
 // 1.replace 该方法可以替换字符，后续常用正则替换
      var str = "ha";
      var newstr = str.replace("h", "t");
      console.log(newstr);

 // 2.valueof() ，返回字符串的原始值，通常在JavaScript内部调用，而不是在代码中显式调用
     console.log(str.valueOf());

~~~



##### 字符串驼峰转化

~~~js
        var str = "wo*Ai*300*qianduan*kaifa*888";
        //    var newstr = "WoAiQianduanKaifa";
        var new_str = ""
        var strArr = str.split("*");
        console.log(strArr);
        for (i = 0; i <= strArr.length - 1; i++) {
            if (isNaN(Number(strArr[i]))) {
                strArr[i] = strArr[i].charAt(0).toUpperCase() + strArr[i].substring(1);
                new_str += strArr[i]
            }

        }


 var newArr = []
        for (var i = 0; i < arr.length; i++) {
            if (newArr.indexOf(arr[i]) === -1) {
                newArr.push(arr[i])
            }
        }
        console.log(newArr)

~~~



### 7.对象

#### 1.什么是对象？

Object类型，我们也称为一个对象，是JavaScript中的引用数据类型。它是一种复合值，它将很多值聚合到一起，可以通过名字访问这些值。对象也可以看做是属性的无序集合，每个属性都是一个名/值对。对象除了可以创建自有属性，还可以通过从一个名为原型的对象那里继承属性。除了字符串、数字、true、false、null和undefined之外，JavaScript中的值都是对象

#### 2.创建对象和访问对象



~~~js
// 1.使用new关键字创建
var person = new Object();
person.name ="赵丽颖";
person.age = 25 ;
person.subject = "戏剧表演";

// 2.使用字面量创建
var person = {
    name:"张艺谋",
    age : 72,
    subject:"电影导演",
}
//1.访问方式 使用 .访问
console.log(person.age);
//2.对象[‘属性名’]
console.log(person["age"])
//3.删除对象 使用delete关键字
delete person.age;
~~~



#### 3.遍历对象

~~~js
var person = {
    name: "zhangsan",
    age: 18
}

for (var personKey in person) {
    // key键  表示对象的属性  person[key] 表示对象的属性值
    var personVal = person[personKey];
    console.log(personKey + ":" + personVal);
}

~~~





### 8.  数据类型梳理

#### 1.基本数据类型  值类型

```js
/*JavaScript中的变量可能包含两种不同数据类型的值：基本数据类型和引用数据类型。

JavaScript中一共有5种基本数据类型：String、Number、 Boolean、Undefined、Null。

基本数据类型的值是无法修改的，是不可变的。

基本数据类型的比较是值的比较，也就是只要两个变量的值相等，我们就认为这两个变量相等。
*/
```

#### 2 引用数据类型

```js
 /*引用类型的值是保存在内存中的对象。

当一个变量是一个对象时，实际上变量中保存的并不是对象本身，而是对象的引用。

当从一个变量向另一个变量复制引用类型的值时，会将对象的引用复制到变量中，并不是创建一个新的对象。

这时，两个变量指向的是同一个对象。因此，改变其中一个变量会影响另一个。

```

####  3.栈和堆的梳理

**1.JavaScript在运行时数据是保存到栈内存和堆内存当中的。**

**2.栈  保存变量和基本类型，堆   是用来保存对象**

**3.声明一个变量时，实际上就是在栈内存中创建了一个空间用来保存变量。**

**4.基本类型  在栈内存中直接保存，引用类型则会在堆内存中保存，变量中保存的实际上对象在堆内存中的地址**

~~~js
var age = 10 ;
var person = {
    name:"赵丽颖",
    age:"30"
}
var oldAge = person.age
~~~



### 9.函数

#### 1.什么是函数？

函数是由一连串的子程序（语句的集合）所组成的，可以被外部程序调用，向函数传递参数之后，函数可以返回一定的值。

通常情况下，JavaScript代码是自上而下执行的，不过函数体内部的代码则不是这样。如果只是对函数进行了声明，其中的代码并不会执行，只有在调用函数时才会执行函数体内部的代码。

这里要注意的是JavaScript中的函数也是一个对象，使用typeof检查一个函数对象时，会返回function。

#### 2.创建函数

1.使用函数对象 创建一个函数 （几乎不用）

~~~js
var 函数名 = new Function("执行语句");
var fun = new Function("console.log('这是我的第一个函数')")
~~~

2.使用函数声明来创建一个对象

```js
function 函数名([形参1，形参2...形参N])
function fun(){
    console.log("这是我的第二个函数")
}
```

3.使用函数表达式来创建一个函数（匿名函数 常用）

```js
var 函数名 = function ([形参1，形参2...形参N]){
    语句....
}
var fun  = function() {
    console.log("这是我的第三个匿名函数");
}

```



#### 3.参数调用

##### **1.无参函数调用**

```js
// 函数声明
var fun  = function() {
    console.log("这是我的第三个函数");
}
// 函数调用 
fun();
```



##### 2.有参函数调用

~~~js
// 函数声明
var sum = function (num1, num2) {
                    // 形参
    var result = num1 + num2;
    console.log("num1 + num2 = " + result);
}

// 函数调用
sum(10, 20);
// 实参
~~~



##### 3.函数参数

+ JS中的所有的参数传递都是按值传递的，也就是说把函数外部的值赋值给函数内部的参数，就和把值从一个变量赋值给另一个变量是一样的，在调用函数时，可以在()中指定实参（实际参数），实参将会赋值给函数中对应的形参
+ 调用函数时，解析器不会检查实参的类型，所以要注意，是否有可能会接收到非法的参数，如果有可能，则需要对参数进行类型的检查，函数的实参可以是任意的数据类型
+ 调用函数时，解析器也不会检查实参的数量，多余实参不会被赋值，如果实参的数量少于形参的数量，则没有对应实参的形参将是undefined
  

##### 4.函数return返回值

*a* + *b*

```js
注意：在函数中return后的语句都不会执行，如果return语句后不跟任何值就相当于返回一个undefined，如果函数中不写return，则也会返回undefined，return后可以跟任意类型的值
```

```js
function sum(num1, num2) {
    return num1 + num2;
}

var result = sum(10, 20);
console.log(result);

```



##### **5.嵌套函数**

嵌套函数：在函数中声明的函数就是嵌套函数，嵌套函数只能在当前函数中可以访问，在当前函数外无法访问。

```js
function fu() {
    function zi() {
        console.log("我是嵌套函数")
    }

    zi();
}

fu();

```



##### 6.立即执行函数

立即执行函数：函数定义完，立即被调用，这种函数叫做立即执行函数，立即执行函数往往只会执行一次。

~~~ js
(function () {
    alert("我是一个匿名函数");
})();

~~~



##### 7.对象中的函数

+ 对象的属性值可以是任何的数据类型，也可以是个函数。

+ 如果一个函数作为一个对象的属性保存，那么我们称这个函数是这个对象的方法，调用这个函数就说调用对象的方法（method）。

+ 注意：方法和函数只是名称上的区别，没有其它别的区别

~~~js
var person = {
    name: "zhangsan",
    age: 18,
    sayHello: function () {
        console.log(name + " hello")
    }
}

person.sayHello();

~~~



##### 8.this指向

解析器在调用函数每次都会向函数内部传递进一个隐含的参数，这个隐含的参数就是this，this指向的是一个对象，这个对象我们称为函数执行的上下文对象，根据函数的调用方式的不同，this会指向不同的对象

- 以函数的形式调用时，this永远都是window
- 以方法的形式调用时，this就是调用方法的那个对象



~~~js
//创建一个全局变量name
var name = "全局变量name";

//创建一个函数
function fun() {
    console.log(this.name);
}

//创建一个对象
var obj = {
    name: "孙悟空",
    sayName: fun
};

//我们希望调用obj.sayName()时可以输出obj的名字而不是全局变量name的名字
obj.sayName();

~~~



#### 4.定时器

JavaScript提供定时执行代码的功能，叫做定时器（timer），主要由`setTimeout()`和`setInterval()`这两个函数来完成。它们向任务[队列](https://so.csdn.net/so/search?q=队列&spm=1001.2101.3001.7020)添加定时任务。

##### **1.setInterval定时器  **

<font size=4 color=red>每隔多少毫秒执行一次代码</font>

```js
var timer=window.setInterval(function(){
     console.log("你好",i)
    i+=1
},2000);

// 清除定时器
window.clearInterval(timer)

// 重置定时器
function reset(){
    //重置定时器，重新给定参数，清除定时器，重新创建定时器
    i=0;
    window.clearInterval(timer);
    timer=window.setInterval(func,2000);
}
```



##### 2.setTimeout延时器

setTimeout(函数，延时时间)

```js
var timer1=window.setTimeout(function (){
    console.log("你好啊！！！");
},3000);
// 清除延时器
window.clearTimeout(timer1)
```



##3.JavaScript高级

### 1.预处理

#### **1.JavaScript的解析和执行过程**

```js
/*javascript是一种描述型的脚本语言，是一种解析语言，由浏览器动态解析，不同种类的浏览器不同
版本的浏览器对于js的解析有着微小的差别，不同浏览器的js解析引擎效率也有高低。
js的执行过程分为两大部分：
第一部分，解析过程，也称预编译期 。主要工作就是对于js的代码中声明的所有变量和函数进行预
处理。需要注意的是，再此进行处理的仅是声明函数，而对于变量的处理仅是声明，并开辟出一块内存
空间，不进行赋值操作。
第二部分，执行过程，在执行过程中，浏览器的js引擎对于每个代码块进行顺序执行，如果有外部
引用的js，且js有相互关联，此时就要注意，不同js的引入顺序，如果声明代码块在调用代码块后调用则
将不会达到预期的效果。
总的来说，JS的执行分为两部分，解析过程和执行过程。解析时按照代码块，一段一段进行解析，
执行时按照代码块顺序逐行执行，解析一个代码块，执行一个代码块。
因为是解释性语言，所以js如果在解析过程有错误，则不会提示，也可以理解为js不会出现编译错
误，但如果出现了运行时错误，出现错误的所有javascript代码将不会继续执行。*/

var num = 10 ;
var num

num = 10;
```



#### 2.预处理

> 预处理：创建一个词法环境（LexicalEnvironment，在后面简写为LE），扫描JS中的用声明的方式 声明的函数，用var定义的变量并将它们加到预处理阶段的词法环境中去。 预处理阶段先读取代码块，不是一行一行的解析执行定义的方法，
>
> 用var 定义的变量，会放到一个 （不同的环境，会有对应的词法环境）词法环境中

``` js
var a = 1; //用var定义的变量，以赋值
var b; //用var定义的变量，未赋值
c = 3; //未定义，直接赋值
function d(){ //用声明的方式声明的函数
console.log('hello');
}
var e = function(){ //函数表达式
console.log('world');
}

```

+ 词法环境

  ```js
  LE{ //此时的LE相当于window
  a:undefined
  b:undefined
  没有c
  d:对函数的一个引用
  e: undefined
  }
  ```

+ 预处理的函数必须是JS中用声明的方式声明的函数（不是函数表达式）。

示例

```js
d();
e();
function d(){//用声明的方式声明的函数
console.log('hello');
}
var e = function(){//函数表达式
console.log('world');
}
```

```js
LE{ //此时的LE相当于window
d:对函数的一个引用
e: undefined
}

// 结果：hello；报错e is not a function。
```



#### 3.命名冲突

变量和函数同名冲突 —— 函数优先，函数是一等公民，在既有函数声明又有变量声明的时候,函数 声明的权重总是高一些，所以最终结果往往是指向函数声明的引用。

```js
console.log(f);
var f = 1;
function f(){
console.log('foodoir');
}

//结果 [Function: f]

```

```js

console.log(f);
function f(){
console.log('foodoir');
}
var f = 1;
// 结果： [Function: f]
```

<font size=4 color=red>变量和函数      同名冲突 —— 后者会覆盖前者</font>

```js
f()
function f(){
console.log('good');
}
function f(){
console.log('hello world');
}

//结果： ‘hello world’
```

```js
var f = 1;
var f = 2;
console.log(f)
//结果 2
```

#### 4.执行阶段

```js
console.log(a); //为什么是undefined？
console.log(b);
console.log(c); //函数在任意地方都可以调用
console.log(d);
var a = 1;
b = 2;
console.log(b);// 2
function c(){
console.log('c');
}
var d = function(){
console.log('d');
}
console.log(d);

```



~~~js
//词法环境
LE{
a:undefined
没有b
c:对函数的一个引用
d:undefined
}

~~~

```js
undefined
报错
function c(){console.log(‘c’);
undefined
```

+ 注释掉上面代码第二行

~~~js
// 1. 在第6行代码执行完，LE中的a的值变为1；
LE{
a:1
没有b
c:对函数的一个引用
d:undefined
}

~~~

~~~js
// 2.第7行代码执行完，LE中就有了b的值（且b的值为2，此时b的值直接变为全局变量）;
LE{
a:1
b:2
c:对函数的一个引用
d:undefined
}

~~~

```js
//3.第10行代码执行完
LE{
a:1
b:2
c:指向函数
d:undefined
}

```

```js
//4.第14行代码执行完，此时

LE{
a:1
b:2
c:指向函数
d:指向函数
}
```



#### 5.函数冲突原则

+ 1.处理函数声明有冲突时，会覆盖。

+ 2 .处理变量声明时有冲突，会忽略。以传入参数的值为准。 

  <font size = 4 color=red>预处理阶段传入参数值一 一对应</font>

```js
function f(a,b){
alert(a);
alert(b);
var b = 100;
function a(){}
}
f(1,2);
LE{
b:2
a:指向函数的引用
arguments：2
}
//arguments，调用函数时实际调用的参数个数

```

```js
// 执行到第6行的时候
LE{
b:2
a:指向定义好的函数
arguments：2
}
//arguments，调用函数时实际调用的参数个数
```

<font size=4 color=red>传入没有参数的值时</font>

```js
function f(a,b){
alert(a);
alert(b);
var b = 100;
function a(){}
}
f(1);

```

~~~js
LE{
b:undefined
a:对函数的一个引用
arguments：1
}


~~~

<font size=4 color=red>没有用var声明的变量，会变成最外部LE的成员，即全局变量</font>

```js
function a(){
function b(){
g = 12;
}
b();
}
a();
console.log(g);//12

```



### 2.作用域

#### 1.什么是作用域？

作用域是在运行时代码中的某些特定部分中变量，函数和对象的可访问性。

换句话说，作用域决定 了代码区块中变量和其他资源的可见性。

例如：

```js
function outFun2() {
var inVariable = "内层变量2";
}
outFun2();//要先执行这个函数，否则根本不知道里面是啥
console.log(inVariable); // Uncaught ReferenceError: inVariable is not undefined
```



从上面的例子可以体会到作用域的概念，变量 inVariable 在全局作用域没有声明，所以在全局作用 域下取值会报错：

+ <font size=4 color=red> 作用域就是一个独立的地盘，让变量不会外泄、暴露出去。</font>

+ <font size=4 color=red>作用域最大的用处就是隔离变量，不同作用域下同名变量不会有冲突。</font>
+ <font size= 4 color=red> ES6 之前 JavaScript 没有块级作用域,只有全局作用域和函数作用域。</font>

ES6 的到来，为我们提供 了‘块级作用域’,可通过新增命令 let 和 const 来体现。

#### 2.全局作用域

在代码中任何地方都能访问到的对象拥有全局作用域，一般来说以下几种情形拥有全局作用域：

##### **1.最外层函数**

**和在最外层函数外面定义的变量拥有全局作用域**

```js
var outVariable = "我是最外层变量"; //最外层变量
function outFun() { //最外层函数
var inVariable = "内层变量";
function innerFun() { //内层函数
console.log(inVariable);
}
innerFun();
}
console.log(outVariable); //我是最外层变量
outFun(); //内层变量
console.log(inVariable); //inVariable is not defined
innerFun(); //innerFun is not defined

```

##### **2.末定义**

**直接赋值的变量自动声明为拥有全局作用域**

```js
function outFun2() {
variable = "未定义直接赋值的变量";
var inVariable2 = "内层变量2";
}
outFun2();//要先执行这个函数，否则根本不知道里面是啥
console.log(variable); //未定义直接赋值的变量
console.log(inVariable2); //inVariable2 is not defined

```

##### **3. window 对象**

**所有window的属性拥有全局作用域**

一般情况下，window 对象的内置属性都拥有全局作用域，例如 window.name、 window.location. 等等。



函数作用域,是指声明在函数内部的变量，和全局作用域相反，局部作用域一般只在固定的代码片段 内可访问到，最常见的例如函数内部。

```js
function doSomething(){
var blogName="浪里行舟";
function innerSay(){
alert(blogName);
}
innerSay();
}
alert(blogName); //脚本错误
innerSay(); //脚本错误
```

##### **4.作用域是分层**

**内层作用域可以访问外层作用域的变量，反之则不行。**

例如：

```js
function fun(a){
    var b = a*2;
    function bar(c){
        consloe.log(a,b,c)
    }
    bar(b*3)
}
fun(2);//2,4,12
//泡泡 a 是全局作用域，有标识符 fun；
//泡泡 b 是作用域 fun，有标识符 a,bar,b；
//泡泡 3 是作用域 bar，仅有标识符 c。
```



**注意的是：块语句（大括号“｛｝”中间的语句），如 if 和 switch 条件语句或 for 和 while 循 环语句，不像函数，它们不会创建一个新的作用域。**

**在块语句中定义的变量将保留在它们已经存在的作 用域中。**

```js
if (true) {
// 'if' 条件语句块不会创建一个新的作用域
var name = 'Hammad'; // name 依然在全局作用域中
}
console.log(name); //  'Hammad'
```

#### **3.块级作用域**

块级作用域可通过新增命令 **let 和 const** 声明，所声明的变量在指定块的作用域外无法被访问。块 级作用域在如下情况被创建：

+ **1.在一个函数内部。**
+ **2.在一个代码块（由一对花括号包裹）内部。**



**<font color=red>块级作用域特点</font>**

##### **1.let/const 关键字**

**并不会被提升到当前代码块的顶部，**

**因此你需要手动将 let/const 声明放置到顶部， 以便让变量在整个代码块内部可用。**

```js
function getValue(condition) {
if (condition) {
let value = "blue";
return value;
} else {
// value 在此处不可用
return null;
}
// value 在此处不可用
}

```

##### **2.禁止重复声明**

如果一个标识符已经在代码块内部被定义，那么在此代码块内使用同一个标识符进行 let 声明就会 导致抛出错误。

例如:

```js
var count = 30;
let count = 40; // Uncaught SyntaxError: Identifier 'count' has already been
declared
```

在本例中， count 变量被声明了两次：一次使用 var ，另一次使用 let 。

因为 let 不能在同一作用域 内重复声明一个已有标识符，此处的 let 声明就会抛出错误。

但如果在嵌套的作用域内使用 let 声明一个 同名的新变量，则不会抛出错误。

```js
var count = 30;
// 不会抛出错误
if (condition) {
let count = 40;
// 其他代码
}

```

##### **3.循环中绑定块级作用域的妙用**

开发者可能最希望实现 for 循环的块级作用域了，因为可以把声明的计数器变量限制在循环内，

例 如，以下代码在 JS 经常见到：

```js
<button>测试1</button>
<button>测试2</button>
<button>测试3</button>
<script type="text/javascript">
var btns = document.getElementsByTagName('button')
for (var i = 0; i < btns.length; i++) {
btns[i].onclick = function () {
console.log('第' + (i + 1) + '个')
}
}

```

我们要实现这样的一个需求: 点击某个按钮, 提示"点击的是第 n 个按钮",此处我们先不考虑事件代理, 万万没想到，点击任意一个按钮，后台都是弹出“第四个”,这是因为 i 是全局变量,执行到点击事件时，此 时 i 的值为 3。那该如何修改，最简单的是用 let 声明 i。

```js
for (let i = 0; i < btns.length; i++) {
btns[i].onclick = function () {
console.log('第' + (i + 1) + '个')
}
}
```



#### 4.作用域链

##### 1.什么是自由变量

首先认识一下什么叫做 自由变量 。如下代码中， console.log(a) 要得到 a 变量，但是在当前的 作用域中没有定义 a（可对比一下 b）。当前作用域没有定义的变量，这成为自由变量 。自由变量的值 如何得到 —— 向父级作用域寻找（注意：这种说法并不严谨，下边会重点解释）。

```js
var a = 100
function fn() {
var b = 200
console.log(a) // 这里的a在这里就是一个自由变量
console.log(b)
}
fn()
```

##### 2 .什么是作用域链?

父级没有自由变量的值？再一层一层向上寻找，直到找到全局作用域还是没找到，就宣布放弃。这种一层 一层的关系，就是作用域链 。

```js
var a = 100
function F1() {
var b = 200
function F2() {
var c = 300
console.log(a) // 自由变量，顺作用域链向父作用域找
console.log(b) // 自由变量，顺作用域链向父作用域找
console.log(c) // 本作用域的变量
}
F2()
}
F1()

```



##### 3.自由变量的值

关于自由变量的值，上文提到要到父作用域中取，其实有时候这种解释会产生歧义。

```js
var x = 10
function fn() {
  console.log(x)//
}
function show(f) {
    var x = 20
  (function() {
f() //10，而不是20
})()
}
show(fn)
```

在 fn 函数中，取自由变量 x 的值时，要到哪个作用域中取？

**要到创建 fn 函数的那个作用域中 取，无论 fn 函数将在哪里调用。**

 所以，不要在用以上说法了。相比而言，用这句话描述会更加贴切:

**要到创建这个函数的那个域” 作用域中取值,这里强调的是“创建”，而不是“调用”，**

切记切记——其实这就是所谓的"静态作用域"。

~~~js

var a = 10
function fn() {
var b = 20
function bar() {
console.log(a + b) //30
}
return bar
}
var x = fn(),
b = 200
x() //bar()

~~~

fn()返回的是 bar 函数，赋值给 x。执行 x()，即执行 bar 函数代码。

取 b 的值时，直接在 fn 作用域 取出。

取 a 的值时，试图在 fn 作用域取，但是取不到，

只能转向创建 fn 的那个作用域中去查找，结果 找到了,所以最后的结果是 30。



### 3.变量提升

#### 1.什么是变量提升？

通常JS引擎会在正式执行之前先进行一次预编译，

在这个过程中，首先将变量声明及函数声明提升 至当前作用域的顶端，然后进行接下来的处理。

(注：当前流行的JS引擎大都对源码进行了编译，由于引 擎的不同，编译形式也会有所差异，我们这里说的预编译和提升其实是抽象出来的、易于理解的概念)。 下面的代码中，我们在函数中声明了一个变量，不过这个变量声明是在if语句块中：



```js
function hoistVariable() {
if (!foo) {
var foo = 5;
}
console.log(foo); // 5
}
hoistVariable();

```

运行代码，我们会发现foo的值是5，大家可能对此不甚理解，如果外层作用域也存在一个foo变 量，就更加困惑了，该不会是打印外层作用域中的foo变量吧？答案是：不会，如果当前作用域中存在此 变量声明，无论它在什么地方声明，引用此变量时就会在当前作用域中查找，不会去外层作用域了。

**那么至于说打印结果，这要提到预编译机制了，经过一次预编译之后，上面的代码逻辑如下：**

```js

// 预编译之后
function hoistVariable() {
var foo;
if (!foo) {
foo = 5;
}
console.log(foo); // 5
}
hoistVariable();
```

是的，引擎将变量声明提升到了函数顶部，初始值为undefined，

自然，if语句块就会被执行，foo 变量赋值为5，下面的打印也就是预期的结果了。



~~~js
var foo = 3;
function fun() {
var foo = foo || 5;
console.log(foo); // 5
}
fun();
~~~

foo || 5这个表达式的结果是5而不是3，

虽然外层作用域有个foo变量，但函数内是不会去引用的， 因为预编译之后的代码逻辑是这样的：

```js
var foo = 3;
// 预编译之后
function hoistVariable() {
var foo;
foo = foo || 5;
console.log(foo); // 5
}
hoistVariable();


```

如果当前作用域中声明了多个同名变量，那么根据我们的推断，它们的同一个**标识符**会被提升至作 用域顶部，其他部分按顺序执行，比如下面的代码：

~~~js
function fun() {
var foo = 3;
{
var foo = 5;
}
console.log(foo); // 5
}
fun()
~~~



由于JavaScript没有块作用域，只有全局作用域和函数作用域，所以预编译之后的代码逻辑为：



~~~js
// 预编译之后
function hoistVariable() {
var foo;
foo = 3;
{
foo = 5;
}
console.log(foo); // 5
}
hoistVariable()
~~~



#### 2.什么是函数提升？

~~~js
function hoistFunction() {
foo(); // output: I am hoisted
function foo() {
console.log('I am hoisted');
}
}
hoistFunction();

~~~

为什么函数可以在声明之前就可以调用，并且跟变量声明不同的是，它还能得到正确的结果，

其实 引擎是把函数声明整个地提升到了当前作用域的顶部，预编译之后的代码逻辑如下：

```js
// 预编译之后
function hoistFunction() {
function foo() {
console.log('I am hoisted');
}
foo(); // output: I am hoisted
}
hoistFunction();

```

相似的，如果在同一个作用域中存在多个同名函数声明，后面出现的将会覆盖前面的函数声明：

~~~js
function hoistFunction() {
function foo() {
console.log(1);
}
foo(); // output: 2
function foo() {
console.log(2);
}
}
hoistFunction();
~~~



对于函数，除了使用上面的函数声明，更多时候，我们会使用函数表达式，下面是函数声明和函数表达 式的对比：

~~~js
// 函数声明
function foo() {
console.log('function declaration');
}
// 匿名函数表达式
var foo = function() {
console.log('anonymous function expression');
};
// 具名函数表达式
var foo = function bar() {
console.log('named function expression');
};
~~~

可以看到，匿名函数表达式，其实是将一个不带名字的函数声明赋值给了一个变量，而具名函数表 达式，则是带名字的函数赋值给一个变量，需要注意到是，这个函数名只能在此函数内部使用。我们也 看到了，其实函数表达式可以通过变量访问，所以也存在变量提升同样的效果。 那么当函数声明遇到函数表达式时，会有什么样的结果呢，先看下面这段代码：



~~~js
function hoistFunction() {
foo(); // 2
var foo = function() {
console.log(1);
};
foo(); // 1
function foo() {
console.log(2);
}
foo(); // 1
}
hoistFunction();

~~~

运行后我们会发现，输出的结果依次是2 1 1，为什么会有这样的结果呢？ 因为JavaScript中的函数是一等公民，函数声明的优先级最高，会被提升至当前作用域最顶端，所以 第一次调用时实际执行了下面定义的函数声明，然后第二次调用时，由于前面的函数表达式与之前的函 数声明同名，故将其覆盖，以后的调用也将会打印同样的结果。上面的过程经过预编译之后，代码逻辑 如下：

~~~js
// 预编译之后
function hoistFunction() {
var foo;
foo = function foo() {
console.log(2);
}
foo(); // 2
foo = function() {
console.log(1);
};
foo(); // 1
foo(); // 1
}
hoistFunction();
~~~

我们也不难理解，下面的函数和变量重名时，会如何执行：

```js
var foo = 3;
function hoistFunction() {
console.log(foo); // function foo() {}
foo = 5;
console.log(foo); // 5
function foo() {}
}
hoistFunction();
console.log(foo); // 3
```

我们可以看到，函数声明被提升至作用域最顶端，然后被赋值为5，而外层的变量并没有被覆盖， 经过预编译之后，

上面代码的逻辑是这样的：

~~~js
// 预编译之后
var foo = 3;
function hoistFunction() {
var foo;
foo = function foo() {};
console.log(foo); // function foo() {}
foo = 5;
console.log(foo); // 5
}
hoistFunction();
console.log(foo); // 3
~~~



所以，函数的优先权是最高的，它永远被提升至作用域最顶部，然后才是函数表达式和变量按顺序 执行，这一点要牢记。





#### 3.为什么要进行提升?

由于第一代JS虚拟机中的抽象纰漏导致的，编译器将变量放到了栈槽内并编入索引，然后在（当前 作用域的）入口处将变量名绑定到了栈槽内的变量。（注：这里提到的抽象是计算机术语，是对内部发 生的更加复杂的事情的一种简化。） 函数提升要了解一下相互递归（就是A函数内会调用到B函数，而B函数也会调用到A函数），函数 提升就是为了解决相互递归的问题，大体上可以解决像ML语言这样自下而上的顺序问题。

~~~js
// 验证偶数
function isEven(n) {
if (n === 0) {
return true;
}
return isOdd(n - 1);
}
console.log(isEven(2)); // true
// 验证奇数
function isOdd(n) {
if (n === 0) {
return false;
}
return isEven(n - 1);
}

~~~

相互递归函数示例：

~~~js
// 验证偶数
function isEven(n) {
if (n === 0) {
return true;
}
return isOdd(n - 1);
}
console.log(isEven(2)); // true
// 验证奇数
function isOdd(n) {
if (n === 0) {
return false;
}
return isEven(n - 1);
}

~~~



如果没有函数提升，而是按照自下而上的顺序，当isEven函数被调用时，isOdd函数还未声明，所 以当isEven内部无法调用isOdd函数。所以Brendan Eich设计了函数提升这一形式，将函数提升至当前 作用域的顶部：

~~~js
// 验证偶数
function isEven(n) {
if (n === 0) {
return true;
}
return isOdd(n - 1);
}
// 验证奇数字
function isOdd(n) {
if (n === 0) {
return false;
}
return isEven(n - 1);
}
console.log(isEven(2)); // true

~~~

这样一来，问题就迎刃而解了。变量提升是人为实现的问题，而函数提升在当初设计时是有目的 的。



#### 4.最佳案例

理解变量提升和函数提升可以使我们更了解这门语言，更好地驾驭它，但是在开发中，我们不应该 使用这些技巧，而是要规范我们的代码，做到可读性和可维护性。 具体的做法是：无论变量还是函数，都必须先声明后使用。下面举了简单的例子：

~~~js
var name = 'Scott';
var sayHello = function(guest) {
console.log(name, 'says hello to', guest);
};
var i;
var guest;
var guests = ['John', 'Tom', 'Jack'];
for (i = 0; i < guests.length; i++) {
guest = guests[i];
// do something on guest
sayHello(guest);
}

~~~

如果对于新的项目，可以使用let替换var，会变得更可靠，可维护性更高：

```js
let name = 'Scott';
let sayHello = function(guest) {
console.log(name, 'says hello to', guest);
};
let guests = ['John', 'Tom', 'Jack'];
for (let i = 0; i < guests.length; i++) {
let guest = guests[i];
// do something on guest
sayHello(guest);
}
/*ES6中的class声明也存在提升，不过它和let、const一样，被约束和限制了，其规定，如果再声明
位置之前引用，则是不合法的，会抛出一个异常。
所以，无论是早期的代码，还是ES6中的代码，我们都需要遵循一点，先声明，后使用。*/
```



##4. JavaScript--->Es6

### 1.箭头函数

~~~js
 // 普通函数 函数声明具名函数 有具体名字的函数就是具名函数

        function fun0(x, y) {
            console.log(x + y);//3
        }
        fun0(1, 2);

        // 表达式声明普通匿名函数
        var fun1 = function (a, b) {
            console.log(a * b);//6
        }
        fun1(2, 3)

        // 箭头函数 
        // 1. 使用箭头替换function,箭头函数是匿名函数
        // 2. 箭头函数，如果函数体，只有一句代码，可以省略花括号
        // 3. 箭头函数，如果只有一个形参可以省略小括号
        /*   var fun2 = (a, b) => {
              console.log(a * b);//15
          }
          fun2(3, 5);
       */
        // 上述代码如下
        // var fun3 = (a, b) => console.log(a * b);//15

        // fun3(3, 5);


        // 第3句解释举例
        var fun2 = a => {
            console.log(a * 5)
        };//15

        fun2(3);


        // 2和3综合 而成的箭头函数
        var fun4 = a => console.log(a * 5);//50
        fun4(10)



        var arr = [1, 2, 3, 4, 5];
        arr.forEach(value => {
            // console.log(value);
        });

        //箭头函数中的this指向不同
        // 在普通函数中，this总是指向调用它的对象，但是箭头函数 本身没有this，
        // 但是它可以捕获其所在上级的this供自己使用
        var subject = "web开发";
        let fun5 = () => {
            this.subject = "javaScript";
            let fun6 = () => {
                console.log(this.subject);//javaScript
            }
            fun6();
        }
        fun5();


        // 普通的函数，当不确定有多少个实参传递的时候，可以使用arguments进行遍历
        // function fun0() {
        //     console.log(arguments);
        // }
        // fun0(1, 2, 43, 4, 34, 34, 34, 2, 7, 8, 9, 3, 3, 2, 0, 3, 5);

        // 箭头函数没有内置对象arguments ，所以我们要用(...形参名 ) 解决参数传递问题,
        let fun7 = (...a) => {
            console.log(a);
        }
        fun7(1, 2, 43, 4, 34, 34, 34, 2, 7, 8, 9, 3, 3, 2, 0, 3, 5);
~~~













## 4.JavaScript--->DOM

### 1.什么是DOM？

#### **1.文档对象模型**

+ **DOM: Document Object Model，全称文档对象模型，简称DOM模型, DOM树。**

+ **它是JS操作网页(HTML文档)的接口API(函数，方法)，（ Application Program Interface应用程序接口）**

+ **它的作用是将网页上各种元素（标签）转为相应的JS对象，从而可以使用JS对象对网页进行各种操作(比如增删查改元素)。**

<font size=4 color=red>DOM树 ：HTML **DOM** 模型被结构化为 **对象树** ：</font>

![image-20201019104459658](assets/910bb72bbde0f438991f02a6cda866d7.png)

通过这个对象模型，JavaScript 获得创建动态 HTML 的所有力量：

+ <font size=4 color=red>HTML DOM 是关于如何获取、更改、添加或删除 HTML 元素的标准。</font>

#### 2.DOM文档节点

**什么是节点？**

节点Node，是构成我们网页的最基本的组成部分，网页中的**每一个**部分都可以称为是一个节点。



比如：html标签、属性、文本、注释、整个文档等都是一个节点。

比如：标签我们称为元素节点、属性称为属性节点、文本称为 文本节点、文档称为文档节点。

节点至少拥有nodeType(节点类型)、nodeName(节点名称)和nodeValue(节点值)这三个基本属性。

节点的类型不同，属性和方法也都不尽相同。

节点：Node——构成HTML文档最基本的单元。

常用**节点属性**分为四类：

**文档节点：整个HTML文档**

文档节点（Document）代表的是整个HTML文 档，网页中的所有节点都是它的子节点。

document对象作为window对象的属性存在的，我们不用获取可以直接使用。

**元素节点：HTML文档中的HTML标签**

HTML中的各种标签都是元素节点（Element），这也是我们最常用的一个节点。

浏览器会将页面中所有的标签都转换为一个元素节点， 我们可以通过document的方法来获取元素节点。

例如：<font size=4 color=red>document.getElementById()</font>，根据id属性值获取一个元素节点对象。


**属性节点：元素的属性**

属性节点（Attribute）表示的是标签中的一个一个的属 性，这里要注意的是属性节点并非是元素节点的子节点，而是元素节点的一部分。可以通过元素节点来获取指定的属性节点。

例如：<font size=4 color=red>元素节点.getAttributeNode("属性名")</font>，根据元素节点的属性名获取一个属性节点对象。(注意：一般不使用)

**文本节点：HTML标签中的文本内容**

文本节点（Text）表示的是HTML标签以外的文本内容，任意非HTML的文本都是文本节点，它包括可以字面解释的纯文本内容。文本节点一般是作为元素节点的子节点存在的。获取文本节点时，一般先要获取元素节点，在通过元素节点获取文本节点。

例如：元素节点.firstChild;，获取元素节点的第一个子节点，一般为文本节点。


![image-20201019115655478](assets/2271dc3f0f61e890fe4cb76817fc6942.png)

其他节点请了解

https://blog.csdn.net/weixin_42472040/article/details/88841675
https://developer.mozilla.org/zh-CN/docs/Web/API/Node/nodeType



### 2.DOM文档操作

#### 1.查找HTML元素



|                  方法                   |             描述             |
| :-------------------------------------: | :--------------------------: |
|      document.getElementById(*id*)      | 通过元素 id 来查找元素。单个 |
|  document.getElementsByTagName(*name*)  |  通过标签名来查找元素。多个  |
| document.getElementsByClassName(*name*) |   通过类名来查找元素。多个   |
| document.getElementsByName('name的值')  |   通过name来查找元素。多个   |
|  document.querySelector('各种选择器')   |      各种选择器   单个       |
| document.querySelectorAll('各种选择器') |       各种选择器  多个       |

~~~js
   // 以下方法不推荐使用
    document.title // 标题
    document.head // 头部
    document.body // 主体
    document.images // 文档上所有的图片
    document.all // 获取文档所有的节点
    document.anchors // 获取锚点。
    document.forms // 获取所有表单
    document.scripts // 获取所有脚本
~~~



#### 2.获取HTML的值

|              方法               | 描述                               |
| :-----------------------------: | ---------------------------------- |
|       元素节点.innerText        | 获取html元素的文本                 |
|       元素节点.innerHTML        | 获取html元素的文本（可以识别标签） |
|    元素节点.属性 （a.href）     | 获取html元素的属性值               |
| 元素节点.getAttribute（属性名） | 获取html元素的属性值               |
|       元素节点.style.样式       | 获取html元素的**行内样式值**       |



#### 3.修改HTML的值和样式

|               方法               | 描述                               |
| :------------------------------: | :--------------------------------: |
|     元素节点.innerText=新值      | 修改html元素的文本                 |
|     元素节点.innerHTML =新值     | 修改html元素的文本（可以识别标签） |
|  元素节点.属性 （a.href）= 新值  | 修改html元素的属性值               |
| 元素节点.setAttribute（属性名，属性值）= | 修改html元素的属性值（可以修改自定义属性，只能获取data开头的） |
|       元素节点.style.样式        | 修改html元素的**行内样式值**       |
|元素.ClassName ="类名"|通过改变元素属性修改（不推荐）|
|  元素.classList.add("类名")   | 给元素添加一个类名 |
| 元素.classList.remove("类名") |    移除一个类名    |






```js
//编写一段兼容性代码，用来设置任意标签的文本内容

<script>
    var a = document.|  元素.classList.add("类名")   | 给元素添加一个类名 |
| 元素.classList.remove("类名") |    移除一个类名    |getElementById("a");
 
    setInnerText(a, "你要打开百度吗？");
    console.log(getInnerText(a));
    /*获取任意标签的内容*/
    function getInnerText(element) {
        // 判断浏览器是否支持textContent,如果支持，则使用textContent获取内容，否则使用innerText获取内容。
        if (typeof element.textContent == "undefined") {
            return element.innerText;
        } else {
            return element.textContent;
        }
    }
    /*设置任意标签的内容*/
    function setInnerText(element, text) {
        // 判断浏览器是否支持textContent,如果支持，则使用textContent设置内容，否则使用innerText设置内容。
        if (typeof element.textContent == "undefined") {
            return element.innerText = text;
        } else {
            return element.textContent = text;
        }
    }
</script>


```



#### 4.修改HTML元素

| 方法 | 描述 |
| :--: | :--: |
|   document.createElement(element)   |   创建 HTML 元素节点。   |
|   document.createAttribute(attribute)   |   	创建 HTML 属性节点。   |
|    document.createTextNode(text)  |  创建 HTML 文本节点。    |
|   元素节点.removeChild(element)   |  删除 HTML 元素。    |
|   元素节点.appendChild(element)   |   	添加 HTML 元素。   |
|   元素节点.replaceChild(element)   |    	替换 HTML 元素。  |
|   元素节点.insertBefore(element)   |    在指定的子节点前面插入新的子节点。  |



案例1：**html空文档创建一个ul列表，然后在该列表中追加4个li标签**

案例2：**html原文档，里边有四个li子元素，删除第一个li，替换最后一个li**



| 方法 | 描述 |
| :--: | :--: |
|  元素节点.parentNode	|  返回元素的父节点。|
|  元素节点.parentElement|  	返回元素的父元素。|
|  元素节点.childNodes	|  返回元素的一个子节点的数组（包含空白文本Text节点）。|
|  元素节点.children	|  返回元素的一个子元素的集合（不包含空白文本Text节点）。|
|  元素节点.firstChild	|  返回元素的第一个子节点（包含空白文本Text节点）。|
|  元素节点.firstElementChild	|  返回元素的第一个子元素（不包含空白文本Text节点）。|
|  元素节点.lastChild	|  返回元素的最后一个子节点（包含空白文本Text节点）。|
|  元素节点.lastElementChild|  	返回元素的最后一个子元素（不包含空白文本Text节点）。|
|  元素节点.previousSibling|  	返回某个元素紧接之前节点（包含空白文本Text节点）。|
|  元素节点.previousElementSibling|  	返回指定元素的前一个兄弟元素（相同节点树层中的前一个元素节点）。|
|  元素节点.nextSibling	|  返回某个元素紧接之后节点（包含空白文本Text节点）。|
|  元素节点.nextElementSibling|  	返回指定元素的后一个兄弟元素（相同节点树层中的下一个元素节点）|



### 3.Dom事件

#### 0.事件的概念

HTML 事件是发生在 HTML 元素上的“事情”。 当在HTML 页面中使用 JavaScript 时,JavaScript 能够“应对”这些事件。 HTML 事件可以是浏览器或用户做的某些事情。比如：点击，移入元素，移出元素，鼠标按下，鼠标弹起，键盘按下，键盘弹起等都是事件。

事件有特征：滞后性，必须等待用户的某种操作，才会响应某种事件。

事件学习过程中一定注意：事件执行的时机。

#### 1.表单事件

| 事件 | 描述 |
| :--: | :--: |
|onblur	|当元素失去焦点时运行脚本。|
|onfocus	|当元素获得焦点时运行脚本。|
|onchange	|当元素改变时运行脚本。|
|oninput	|当元素获得用户输入时运行脚本。|
|oninvalid	|当元素无效时运行脚本。|
|onselect	|当选取元素时运行脚本。|
|onsubmit	|当提交表单时运行脚本|

<font size= 4 color=red>通标签默认情况下无法支持输入操作，通过全局属性contenteditable设置成true，就可以支持输入操作了，并且会支持oninput事件</font>

注意：控制form的onsumit事件去实现。

​    这种实现方式有个前提：form中的button必须是提交按钮。

提交表单的两种方式

1. 给form中的button绑定onclick事件去实现。

2. 控制form的onsumit事件去实现。

     这种实现方式有个前提：form中的button必须是提交按钮。

```html
 <button type="submit">登录2</button>
// button的type默认值是submit，表示是提交按钮, type=button普通按钮 

    <p>input输入，oninput表示用户在输入框中输入文本时执行，哪些元素才能输入? input,textarea等。p,div,span,section等这些普</p>

    <!-- oninput事件属性，事件属性后对应的值称为：事件处理程序handler，是真正业务逻辑  this表示当前操作的元素，即input, 实参：实际参数，表示传递过去的参数。-->
    <input type="text" oninput="input(this)" />

    <div contenteditable="true" oninput="input2()">div元素默认情况下无法支持用户输入数据</div>

```



#### 2.窗口事件



| 事件 | 描述 |
| :--: | ---- |
|onload	|当文档加载之后运行脚本。|
|onresize|	当调整窗口大小时运行脚本。|
|onblur	|当窗口失去焦点时运行脚本。|
|onfocus	|当窗口获得焦点时运行脚本|



#### 3.鼠标事件

|属性|	描述|
| :--: | :--: |
|onclick	|当单击鼠标时运行脚本。|
|ondblclick|	当双击鼠标时运行脚本。|
|onmousedown	|当按下鼠标按钮时运行脚本。|
|onmouseup|	当松开鼠标按钮时运行脚本。|
|onmousemove	|当鼠标指针移动时运行脚本。|
|onmouseover|	当鼠标指针移至元素之上时运行脚本，不可以阻止冒泡。|
|onmouseout|	当鼠标指针移出元素时运行脚本，不可以阻止冒泡。|
|onmouseenter|	当鼠标指针移至元素之上时运行脚本，可以阻止冒泡。|
|onmouseleave|	当鼠标指针移出元素时运行脚本，可以阻止冒泡。|
|onmousewheel|	当转动鼠标滚轮时运行脚本。|
|onscroll|	当滚动元素的滚动条时运行脚本。|



#### **4.键盘事件**

|    事件    |                     描述                     |
| :--------: | :------------------------------------------: |
| onkeydown  |      键盘按下（如果不松手，会一直执行）      |
|  onkeyup   |             键盘弹起（按下弹起）             |
| onkeypress | 键盘按下 不松手执行 （按压的过程，没有弹起） |
|            |      onkeypress =  onkeydown + onkeyup       |



#### 5.拖拽事件

|    事件     |                 描述                 |
| :---------: | :----------------------------------: |
| ondragstart |       当用户开始拖动元素时发生       |
|   ondrag    |          当元素被拖动时发生          |
|  ondragend  |       当用户完成拖动元素时发生       |
| ondragenter |   当被拖动的元素进入放置目标时发生   |
| ondragover  |   当被拖动的元素在放置目标上时发生   |
| ondragleave |   当被拖动的元素离开放置目标时发生   |
|   ondrop    | 当被拖动的元素被放在放置目标上时发生 |
|             |                                      |

<font size=4 color=red>event.preventDefault</font>

阻止事件的默认行为



#### 6.Event对象

##### 1.Event 对象

代表事件的状态，比如事件在其中发生的元素、键盘按键的状态、鼠标的位置、鼠标按钮的状态。

   // 1.event 就是一个事件对象 写到我们事件侦听函数的小括号里面

​    // 2.事件对象只有事件执行才会存在 ，它是系统给我们自动创建的 不用我们传递实参

​    // 3.事件对象 是事件执行后一系列相关数据的集合 跟事件相关的 比如鼠标点击里面包含了鼠标信息 鼠标坐标 ，键盘事件里面就包含了键盘事件的信息 key键值

​    // 4.事件对象名称可以自己命名 比如event、evt、e

​    // 5.事件对象也有兼容性问题 ie678 通过window.event 兼容性写法 e = e || window.event

 事件对象本身的获取存在兼容问题：

1. 标准浏览器中是浏览器给方法传递的参数，只需要定义形参 e 就可以获取到。

2. 在 IE6~8 中，浏览器不会给方法传递参数，如果需要的话，需要到 window.event 中获取查找。

3. 兼容性的写法 e=e || window.event

   ~~~js
   <script>
    
       window.onload = function(){
           var Div = document.getElementById('div1');
           document.onmousemove = function(ev){
               var ev = ev||event;//处理兼容性
               Div.style.left = ev.clientX + 'px';
               Div.style.top = ev.clientY + 'px';
           }
       }
    
   </script>
   ~~~



##### 2.鼠标事件对象

|     事件对象      |                          描述                          |
| :---------------: | :----------------------------------------------------: |
| clientX ，clientY |         鼠标对于浏览器窗口可视区的x坐标和y坐标         |
|    pageX,pageY    |              鼠标对于页面文档的x和y的坐标              |
| screenX，screenY  |               鼠标对于电脑屏幕的x和y坐标               |
|   event.button    | 0 表示鼠标左键         1 表示鼠标中间   2 表示鼠标右键 |
|keyCode|键盘键值|
|e.target|返回的是触发事件的对象(元素)|
|this|返回的是绑定事件的对象(元素)|
|e.type|返回绑定事件类型|
|e.preventDefault()|阻止事件的默认行为|
|||

[ Event对象详解 参考文档](https://blog.csdn.net/weixin_43942304/article/details/108326613?ops_request_misc=%7B%22request%5Fid%22%3A%22165864609716782184632025%22%2C%22scm%22%3A%2220140713.130102334..%22%7D&request_id=165864609716782184632025&biz_id=0&utm_medium=distribute.pc_search_result.none-task-blog-2~all~top_click~default-1-108326613-null-null.142^v33^control,185^v2^control&utm_term=event对象&spm=1018.2226.3001.4187)



### 4.事件流

#### 1.DOM发展

DOM的发展，目前有4个阶段，分别DOM0, DOM1， DOM2, DOM3。

//DOM1一般只有设计规范没有具体实现，所以一般跳过。

// DOM3级事件在DOM2级事件的基础上添加了更多的事件类型，如焦点事件  blur、focus，键盘事件keydown、keypress

**比较重要的阶段DOM0和DOM2**

~~~js
    <button onclick="fun1();fun2();">DOM0绑定事件</button>
    <button id="btn"></button>
     // 1. DOM0第一种绑定事件方法
    // 直接在标签中控制事件属性，(不建议使用)原因：影响页面的html结构，不利于代码维护 
       
      // 2. DOM0第二种绑定事件方法
      // 通过此形式绑定的事件，由于onclick是一个事件属性，属性有个特征：多次赋值，最后一次有效，所以这样的绑定只有最后的事件处理程序fun2会执行。
      var btn = document.querySelector("#btn2");
      btn.onclick = function(){  };
       // DOM0事件移除     btn.onclick = null;


/ DOM2事件绑定通过addEventListener添加事件监听，可以多次绑定不同类型的事件，且每个事件类型都有效。addEventListener()在低版本浏览器中不支持。
  var btn = document.querySelector("#btn");
   btn.addEventListener("click", function () {
        console.log("btn点击了。");
  });
/移除事件监听   btn3.removeEventListener("click", clickMe);

~~~



#### 2.事件流分类：

<font size=4 color=red>**在给多个嵌套元素同时绑定事件时，事件执行的顺序就是事件流。**</font>

##### 

**1.*事件冒泡**是由IE开发团队提出来的，**事件开始时由最具体的元素（文档中嵌套层次最深的那个节点）接收，然后逐级向上传播执行。就像冒泡一样**（从内层向外层执行）

2.**事件捕获 ** 由网景公司 团队提出来的  **事件是先由最上一级的节点先接收，然后向下传播到具体的节点。**

（从外边向内层执行 “挖洞”）

**3.事件流三个阶段：事件捕获阶段，处于目标阶段，事件冒泡阶段**



![img](assets/20160213232257842.png)

~~~js
         // DOM0的事件绑定：即事件属性。它只支持冒泡型事件
        // e.cancelBubble = true; event.stopPropagation
         // DOM2通过addEventListener()这个API，也可以支持冒泡型事件流。
        // 参数1：事件类型    参数2：回调函数     参数3：false默认值表示冒泡型事件流，true表示捕获型事件流
        // event.stopPropagation  Propagation传播，用来阻止事件传播。
        // 即可以阻止捕获型事件流，也可以阻止冒泡型事件
		//阻止事件传播：event.stopPropagation()推荐,或者：event.cancelBubble = true
		//阻止元素默认行为：event.preventDefault()推荐，或者e.returnValue = false，
		// 或者低版本的IE浏览器：return false
~~~



#### 3.事件委托（代理）

事件委托是利用事件的冒泡原理来实现的， 

 **两种使用场景：**

​    \1. 存在的元素它自己不想绑定事件，想让其他元素（只在是存在的元素即可）帮它绑带

​    \2. 元素还不存在，所以无法给不存在的元素绑定事件，只能委托其他元素帮它绑定事件。

~~~js

  // 事件委托：张三委托李四，目的让李四帮他去干活。不存在的元素委托存在的元素，让存在的元素帮它去绑定事件的操作，就叫事件委托。
  //如：li标签不存在，但它的父元素ul已经在文档上存在了，站在li标签的角度，li标签就可委托它的父元素ul帮它帮定事件。如果站在ul的角度，ul代理了li帮它绑定事件，称为事件代理。
   var ul = document.querySelector("ul");
        ul.onclick = function(e){
            console.log("给ul绑定的事件")
            console.log(e.target.tagName)
            // 判断用户点击是否是LI标签。
            if(e.target.tagName==="LI"){
                alert("你点击了li")
                var index = e.target.getAttribute("index")
                if(index==1){
                    alert("你点击是第2li")
                }
            }
        }

        var li = document.createElement("li");
        li.textContent = "我是第2个li"
        li.setAttribute("index", 1)
        ul.appendChild(li)
~~~



### 5.坐标位置偏移量

#### 1.鼠标位置

|            事件对象             |                   描述                    |
| :-----------------------------: | :---------------------------------------: |
|      e.clientX，e.clientY       |    鼠标对于浏览器窗口可视区的x和y坐标     |
|         e.pageX,e.pageY         |       鼠标对于页面文档的x和y的坐标        |
|       e.screenX,e.screenY       |        鼠标对于电脑屏幕的x和y坐标         |



#### 2.元素坐标位置

|            事件对象             |                             描述                             |
| :-----------------------------: | :----------------------------------------------------------: |
| 元素.offsetLeft, 元素.offsetTop |           可以获得元素距离有定位的最近父元素的位置           |
|    clientWidth，clientHeight    | 网页可见区域高，clientHeight：包括padding但不包括border、滚动条、margin的元素的高度 |
|    .scrollTop ，.scrollLeft     |         滚动条向下滚动的距离,  滚动条向左滚动的距离          |
|   offsetWidth ，offsetheight    |                    网页/元素可见的宽度值                     |













## 5.JavaScript--->BOM

### **1.BOM基础**

#### **1.什么是BOM?**

BOM：Brower Object Model浏览器对象模型。JavaScript BOM 主要用来操作浏览器。比如创建新页面、弹出对话框、设置定时器、检测浏览器、获取URL信息等。但浏览器对象模型尚无正式标准。

#### 2.BOM和DOM的比较

DOM （Document Object Model文档对象模型） 是一套操作HTML标签的API，已被标准化。
BOM 是一套操作浏览器的API，未标准化。
可以理解成 DOM 只是 BOM 中的一部分。

#### 4.常见的BOM对象！

window：代表整个浏览器窗口（window是BOM中的一个对象，并且是顶级的对象）
navigator：代表浏览器当前的信息，通过navigator我们可以获取用户使用的是什么浏览器
location：代表浏览器当前的地址信息，通过location我们可以获取或者设置URL信息
history：代表浏览器的历史信息，通过history我们可以实现前进/刷新/后退操作
screen：代表计算机屏幕信息



#### 5.window对象

~~~js
window.alert('提示信息')
window.confirm("确认信息")
window.prompt("弹出输入框")
window.open("url地址"，'打开的方式（可以是-self或-black）'，'新窗口的大小'）
window.close() 关闭当前的网页。 注：存在兼容性问题
window.moveTo() 移动当前窗口
window.resizeTo() 调整当前窗口的尺寸
~~~



#### 6.window 尺寸

~~~js
/*
有三种方法能够确定浏览器窗口的尺寸。
对于Internet Explorer、Chrome、Firefox、Opera 以及 Safari：
window.innerHeight - 浏览器窗口的内部高度(包括滚动条)，浏览器可视区域的高
window.innerWidth - 浏览器窗口的内部宽度(包括滚动条)，浏览器可视区域的宽
对于 Internet Explorer 8、7、6、5：
document.documentElement.clientHeight
document.documentElement.clientWidth
或者
document.body.clientHeight
document.body.clientWidth
~~~







#### 7.浅谈URL

**URL： Uniform Resource Locator，统一资源定位器， 访问网络的地址（IP，域名）**
**URI： Uniform Resource Identifier，统一资源标识符**

```js
URI>URL   URL是URI的子集

URI/URL格式：
[协议名]://[用户名]:[密码]@[服务器地址]:[服务器端口号]/[路径]?[查询字符串]#[片段ID]

服务器地址（主机）：就是IP地址 + 端口号。

公网：不需要用户名，密码，端口号默认80，必须省略

协议名：http, https, ftp, file

了解一下协议：
http：是一种通讯协议。超文本传输协议。
https：其中的s（safe）表示安全，安全的超文本传输协议
ftp：文件传输协议
file：文件协议
TCP/IP协议
UDP：断点续传协议
.....

域名：方便记忆，它是在IP地址的基础，通过DNS解析成域名。可以把域名理解成IP地址的别名
本地的服务器（Open With Live Server）默认的IP址地：127.0.0.1,默认域名：localhost，当然也可以用本机的IP地址去访问本地HTML文档。

IP         域名
127.0.0.1  localhost
39.156.66.18  www.baidu.com

如何得到一个域名下的IP地址：
1. win+R打开运行框， 输入cmd回车，打开DOS窗口。
2. 在DOS窗口中输入ipconfig命令，回车即可以拿本地IP地址。
3. 在DOS窗口中输入ping 域名，回车即可以拿到远程的IP地址。

```

#### 8.location对象

<font size=4 color=red>Location对象中封装了浏览器的地址栏的信息   获得当前页面的地址 (URL)，并把浏览器重定向到新的页面,在编写时可不使用 window 这个前缀</font>

##### 1.常用属性

~~~js
/*
location.herf = 'url地址'
location.hash 返回#号后面的字符串，不包含散列，则返回空字符串。
location.host 返回服务器名称和端口号
location.pathname 返回目录和文件名。 /project/test.html
location.search 返回?号后面的所有值。
location.port 返回URL中的指定的端口号，如URL中不包含端口号返回空字符串
location.portocol 返回页面使用的协议。 http:或https:
*/
~~~

##### 2.常用方法

~~~js
location.assign("https://www.baidu.com");
//assign()：用来跳转到其它的页面，作用和直接修改location一样

location.reload(true);
//reload()：用于重新加载当前页面，作用和刷新按钮一样，如果在方法中传递一个true，作为参数，则会强制清空缓存刷新页面

location.replace("https://www.baidu.com");
// replace()：可以使用一个新的页面替换当前页面，调用完毕也会跳转页面，它不会生成历史记录，不能使用回退按钮回退
~~~



#### 9.navigator对象

<font size=4 color=red>window.navigator 对象包含有关访问者浏览器的信息。History对象可以用来操作浏览器向前或向后翻页，在编写时可不使用 window 这个前缀。</font>



~~~js

/*
navigator.userAgent：浏览器设定的User-Agent字符串。
navigator.platform：操作系统类型；
navigator.appCodeName：浏览器代号；
navigator.appName：浏览器名称；
navigator.appVersion：浏览器版本；
navigator.language：浏览器设置的语言；
navigator.systemLanguage：浏览器系统语言；
navigator.cookieEnabled：浏览器是否启用了cookie；
其中userAgent是最常用的属性，用来完成浏览器判断。

~~~

#### 10.histoty对象

~~~js
console.log(history);           //输出history对象
console.log(history.length);    //可以获取到当成访问的链接数量
history.back();  // back()：可以回退到上一个页面，作用和浏览器的回退按钮一样
history.forward(); // forward()：可以跳转到下一个页面，作用和浏览器的前进按钮一样


~~~

<font size=4 color=red>history.go()</font>

go()：可以用来跳转到指定的页面，它需要一个整数作为参数

- 1：表示向前跳转一个页面，相当于forward()
- 2：表示向前跳转两个页面
- -1：表示向后跳转一个页面，相当于back()
- -2：表示向后跳转两个页面
