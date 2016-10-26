#JavaScript 作用?#

    1. HTML 定义了网页的内容
    2. CSS 描述了网页的布局
    3. JavaScript 网页的行为

#&lt;script> 标签#
<style>
	table.dataintable {border: 1px solid #aaa;border-collapse: collapse; margin-top:10px;width: 100%;}
	.html5_new{color:#008000;font-weight:bold;}
	.deprecated{color:#ff0000;}
</style>

###必选的属性###
<table class="dataintable">
	<tr><th style="width:20%;">属性</th><th style="width:20%;">值</th><th style="width:60%;">描述</th></tr>
	<tr><td>type</td><td><i>MIME-type</i></td><td>指示脚本的 MIME 类型。</td></tr>
</table>

###可选的属性###
<table class="dataintable">
	<tr><th style="width:20%;">属性</th><th style="width:20%;">值</th><th style="width:60%;">描述</th></tr>
	<tr><td class="html5_new">async</td><td>async</td><td>规定异步执行脚本（仅适用于外部脚本）。</td></tr>
	<tr><td>charset</td><td><i>charset</i></td><td>规定在外部脚本文件中使用的字符编码。</td></tr>
	<tr><td>defer</td><td>defer</td><td>规定是否对脚本执行进行延迟，直到页面加载为止。</td></tr>
	<tr><td>language</td><td><i>script</i></td><td><span class="deprecated">不赞成使用。</span>规定脚本语言。请使用 type 属性代替它。</td></tr>
	<tr><td>src</td><td><i>URL</i></td><td>规定外部脚本文件的 URL。</td></tr>	
	<tr><td>xml:space</td><td>preserve</td><td>规定是否保留代码中的空白。</td></tr>
</table>

###&lt;script> 标签支持 HTML 中的全局属性###

<table class="dataintable">
	<tr><th style="width:35%;">属性</th><th>描述</th></tr>
	<tr><td>accesskey</td><td>规定激活元素的快捷键。</td></tr>
	<tr><td>class</td><td>规定元素的一个或多个类名（引用样式表中的类）。</td></tr>
	<tr><td class="html5_new">contenteditable</td><td>规定元素内容是否可编辑。</td></tr>

	<tr><td class="html5_new">contextmenu</td><td>规定元素的上下文菜单。上下文菜单在用户点击元素时显示。</td></tr>

	<tr><td class="html5_new">data-*</td><td>用于存储页面或应用程序的私有定制数据。</td></tr>
	<tr><td>dir</td><td>规定元素中内容的文本方向。</td></tr>
	<tr><td class="html5_new">draggable</td><td>规定元素是否可拖动。</td></tr>

	<tr><td class="html5_new">dropzone</td><td>规定在拖动被拖动数据时是否进行复制、移动或链接。</td></tr>

	<tr><td class="html5_new">hidden</td><td>规定元素仍未或不再相关。</td></tr>
	<tr><td>id</td><td>规定元素的唯一 id。</td></tr>
	<tr><td>lang</td><td>规定元素内容的语言。</td></tr>
	<tr><td class="html5_new">spellcheck</td><td>规定是否对元素进行拼写和语法检查。</td></tr>
	<tr><td>style</td><td>规定元素的行内 CSS 样式。</td></tr>
	<tr><td>tabindex</td><td>规定元素的 tab 键次序。</td></tr>
	<tr><td>title</td><td>规定有关元素的额外信息。</td></tr>
	<tr><td class="html5_new">translate</td><td>规定是否应该翻译元素内容。</td></tr>
</table>


#JavaScript 字面量#

> 在编程语言中，一个字面量是一个常量，如 3.14。


* 数字（Number）字面量 可以是整数或者是小数，或者是科学计数(e)。
>     3.14
>     1001
>     123e5

> 表达式字面量 用于计算：

>     5 + 6
>     5 * 10


* 字符串（String）字面量 可以使用单引号或双引号 be written with double or single quotes:
>     "John Doe"
>     'John Doe'


* 数组（Array）字面量 定义一个数组：[40, 100, 1, 5, 25, 10]

* 对象（Object）字面量 定义一个对象：{firstName:"John", lastName:"Doe", age:50, eyeColor:"blue"}

* 函数（Function）字面量 定义一个函数：function myFunction(a, b) { return a * b;}


#JavaScript 变量#

>变量可以通过变量名访问。在指令式语言中，变量通常是可变的。字面量是一个恒定的值。 

>     变量是一个名称。字面量是一个值。

* Value = undefined

> 在计算机程序中，经常会声明无值的变量。未使用值来声明的变量，其值实际上是 undefined。

> 在执行过以下语句后，变量 carname 的值将是 undefined：

>     var carname;

* 重新声明 JavaScript 变量

> 如果重新声明 JavaScript 变量，该变量的值不会丢失：

> 在以下两条语句执行后，变量 carname 的值依然是 "Volvo"：

>     var carname="Volvo";
>     var carname;



#JavaScript 数据类型#
	
> 字符串（String）、数字(Number)、布尔(Boolean)、数组(Array)、对象(Object)、空（Null）、未定义（Undefined）。

* JavaScript 数组

>下面的代码创建名为 cars 的数组：

>     var cars=new Array();
>     cars[0]="Saab";
>     cars[1]="Volvo";
>     cars[2]="BMW";

> 或者 (condensed array):

>     var cars=new Array("Saab","Volvo","BMW");

> 或者 (literal array):

>     var cars=["Saab","Volvo","BMW"]; 

> **数组下标是基于零的，所以第一个项目是 [0]，第二个是 [1]，以此类推。**


* JavaScript 对象

> 对象由花括号分隔。在括号内部，对象的属性以名称和值对的形式 (name : value) 来定义。属性由逗号分隔：

>     var person={firstname:"John", lastname:"Doe", id:5566};

> 上面例子中的对象 (person) 有三个属性：firstname、lastname 以及 id。

> 空格和折行无关紧要。声明可横跨多行：

>     var person={
>         firstname : "John",
>         lastname  : "Doe",
>         id        :  5566
>     };

> 对象属性有两种寻址方式：

>     name=person.lastname;
>     name=person["lastname"]; 

* Undefined 和 Null

> **Undefined 这个值表示变量不含有值。可以通过将变量的值设置为 null 来清空变量。**


* JavaScript 数据类型

> 在 JavaScript 中有 7 种不同的数据类型

>     string
>     number
>     boolean
>     object   （3种对象类型：Object，Date，Array）
>     function
> 
>     //不包含任何值的数据类型：
>     null
>     undefined
    
#向未声明的 JavaScript 变量分配值

> 如果您把值赋给尚未声明的变量，该变量将被自动作为全局变量声明。

> **或者描述为**

> 变量声明是如果不使用 var 关键字，那么它就是一个全局变量，即便它在函数内定义。

> 这条语句：

>     carname="Volvo";

> 将声明一个全局变量 carname，即使它在函数内执行。

#JavaScript 变量生命周期#

* JavaScript 变量生命周期在它声明时初始化。

* 局部变量在函数执行完毕后销毁。

* 全局变量在页面关闭后销毁。

#JavaScript 作用域#

* 函数参数

	> 函数参数只在函数内起作用，是局部变量。

* HTML 中的全局变量

	> 在 HTML 中, 全局变量是 window 对象: 所有数据变量都属于 window 对象。


* 全局变量，或者函数，可以覆盖 window 对象的变量或者函数。
* 局部变量，包括 window 对象可以覆盖全局变量和函数。

#JavaScript 事件#

>&lt;button onclick='getElementById("demo").innerHTML=Date()'>The time is?&lt;/button>

**为什么可以省略document？**


###1. 阻止默认事件###

	function stopDefault(e) {
		if(e && e.preventDefault )
	   		e.preventDefault();
	    else
	   		window.event.returnValue = false;
	    return false;
	}


###2. 阻止事件冒泡###

	function stopBubbling(evt) {
 		var e = evt? evt: window.event;
 		if (window.event) {
  			e.cancelBubble=true; // ie下阻止冒泡
 		} else {
  			e.stopPropagation(); // 其它浏览器下阻止冒泡
 		}
	}


#JavaScript typeof, null, 和 undefined##

	typeof "John"                // 返回 string
	typeof 3.14                  // 返回 number
	typeof false                 // 返回 boolean
	typeof [1,2,3,4]             // 返回 object
	typeof {name:'John', age:34} // 返回 object 


**Undefined 和 Null 的区别**
	
	typeof undefined             // undefined
	typeof null                  // object
	null === undefined           // false
	null == undefined            // true


#JavaScript 运算符#

**规则: 如果把数字与字符串相加，结果将成为字符串！**

**一元运算符 \+**

> Operator + 可用于将变量转换为数字：

>     var y = "5";      // y 是一个字符串
>     var x = + y;      // x 是一个数字 

#JavaScript 正则表达式#

> str.search(patt)               //找到返回位置，找不到返回-1

> string.replace(patt, "sth");   //默认匹配一次停止，全部替换加修正符g

> regexp.test(string);           //字符串中含有匹配的文本，则返回 true，否则返回 false。 

> regexp.exec(string);           //返回匹配的一个结果一个数组，如果未匹配，则返回值为 null。

> string.match(regexp);          //返回匹配的所有结果一个数组，如果未匹配，则返回值为 null。

>     非全局标识g时候，等同于exec，因此exec也略显多余？？？     

> string.split(separator,limit); //转成数组

>      string.split();           //整个字符串作为数组元素
>      string.split("");         //每个字符作为数组元素

> regexp.compile(patt[, flags]); //比直接赋值效率高？？？，flags是修正符：g、i、m

    注意：当使用构造函数创造正则对象时，需要常规的字符转义规则（在前面加反斜杠 \）。比如，以下是等价的：

    var re = new RegExp("\\w+");
    var re = /\w+/;



#JavaScript 调试#

* 设置断点

	在调试窗口中，你可以设置 JavaScript 代码的断点。

	在每个断点上，都会停止执行 JavaScript 代码，以便于我们检查 JavaScript 变量的值。
	
	在检查完毕后，可以重新执行代码（如播放按钮）。

* debugger 关键字

	debugger 关键字用于停止执行 JavaScript，并调用调试函数。
	
	这个关键字与在调试工具中设置断点的效果是一样的。
	
	如果没有调试可用，debugger 语句将无法工作。



#JavaScript 变量提升#


> JavaScript 中，函数及变量的声明都将被提升到函数的最顶部。变量可以在使用后声明，也就是变量可以先使用再声明。

>>注意：只有声明的变量会提升，初始化的不会。

#JavaScript 严格模式(use strict)#

> "use strict";
###
>     不允许使用未声明的变量；
>     不允许删除变量或对象；
>     不允许删除函数；
>     不允许变量重名；                             //function x(p1, p1) {}; 
>     不允许使用八进制；                           //var x = 010; 
>     不允许使用转义字符；                         //var x = \010; 
>     不允许对只读属性赋值；
>         var obj = {}; 
>         Object.defineProperty(obj, "x", {value:0, writable:false});
>         obj.x = 3.14;

>     不允许对一个使用getter方法读取的属性进行赋值；
>         var obj = {get x() {return 0} };
>         obj.x = 3.14;

>     不允许删除一个不允许删除的属性；              //delete Object.prototype;
>     不允许使用with语句；
>     不允许用 "eval", "arguments"关键字作变量名；
>     不允许调用在作用域 eval() 创建的变量；        //eval ("var x = 2"); alert (x);
>     禁止this关键字指向全局对象；
>         function f(){
>         	return !this;
>         } 
>         // 返回false，因为"this"指向全局对象，"!this"就是false

>         function f(){ 
>         	"use strict";
>         	return !this;
>         } 
>         // 返回true，因为严格模式下，this的值为undefined，所以"!this"为true。

>     不允许使用保留关键字作变量名；为了向将来Js的新版本过渡，严格模式新增了一些保留关键字：
>         implements
>         interface
>         let
>         package
>         private
>         protected
>         public
>         static
>         yield


#JavaScript 使用误区#
>     var x = 0;
>     if (x == 10) //false
>     if (x = 10)  //true
>     
> ###
> 
>     var x = 10;
>     var y = "10";
>     if (x == y) 
>     if (x === y) 
>     
> ###
> 
>     switch 语句会使用恒等计算符(===)进行比较:
>     var x = 10;
>     switch(x) {
>         case 10: alert("Hello");    //会弹出
>     } 
>     switch(x) {
>         case "10": alert("Hello");  //不会弹出
>     } 
>     
> ###  
> 
>     浮点型数据使用注意事项
>     var x = 0.1;
>     var y = 0.2;
>     var z = x + y;  // z 的结果为 0.3
>     if (z == 0.3)   // 返回 false
>     var z = (x * 10 + y * 10) / 10;  // z 的结果为 0.3
>     
###    

> 字符串断行需要使用反斜杠(\\)
> 
> JavaScript 默认是在代码的最后一行自动结束, 可以省略分号。
> 
> 由于 return 是一个完整的语句，所以 JavaScript 将关闭 return 语句。 
> 注意：不用对 return 语句进行断行。  

###

> Array使用数字和名字来索引

>     var person = ['number key 0', 'number key 1'];
>     person["firstName"] = "John";
>     person["lastName"]  = "Doe";
>     person["age"]       = 46;
>     //注意person.length 返回 2，名字索引被当作对象属性
>     var x = person.length; 

> 检测对象是否存在(必须先判断是否定义了)

>     if (typeof myObj !== "undefined" && myObj !== null) 

###

> 程序块作用域

>     //在每个代码块中 JavaScript 不会创建一个新的作用域，一般各个代码块的作用域都是全局的。
>     //以下代码的的变量 i 返回 10，而不是 undefined：
>     for (var i = 0; i < 10; i++) {
>         // some code
>     }
>     return i;


#JavaScript 保留关键字#

Javascript 的保留关键字不可以用作变量、标签或者函数名。有些保留关键字是作为 Javascript 以后扩展使用。
<table class="reference">
	<tr> <td>abstract</td> <td>arguments</td> <td>boolean</td> <td>break</td> <td>byte</td> </tr>
	<tr> <td>case</td> <td>catch</td> <td>char</td> <td>class*</td> <td>const</td> </tr> 
	<tr> <td>continue</td> <td>debugger</td> <td>default</td> <td>delete</td> <td>do</td> </tr>
	<tr> <td>double</td> <td>else</td> <td>enum*</td> <td>eval</td> <td>export*</td> </tr> 
	<tr> <td>extends*</td> <td>false</td> <td>final</td> <td>finally</td> <td>float</td> </tr>
	<tr> <td>for</td> <td>function</td> <td>goto</td> <td>if</td> <td>implements</td> </tr>
	<tr> <td>import*</td> <td>in</td> <td>instanceof</td> <td>int</td> <td>interface</td> </tr>
	<tr> <td>let</td> <td>long</td> <td>native</td> <td>new</td> <td>null</td> </tr>
	<tr> <td>package</td> <td>private</td> <td>protected</td> <td>public</td> <td>return</td> </tr>
	<tr> <td>short</td> <td>static</td> <td>super*</td> <td>switch</td> <td>synchronized</td> </tr>
	<tr> <td>this</td> <td>throw</td> <td>throws</td> <td>transient</td> <td>true</td> </tr>
	<tr> <td>try</td> <td>typeof</td> <td>var</td> <td>void</td> <td>volatile</td> </tr>
	<tr> <td>while</td> <td>with</td> <td>yield</td> <td></td> <td></td> </tr>
</table>

#JavaScript 对象、属性和方法#
您也应该避免使用 JavaScript 内置的对象、属性和方法的名称作为 Javascript 的变量或函数名：
<table class="reference">
	<tr> <td>Array</td> <td>Date</td> <td>eval</td> <td>function</td> <td>hasOwnProperty</td> </tr>
	<tr> <td>Infinity</td> <td>isFinite</td> <td>isNaN</td> <td>isPrototypeOf</td> <td>length</td> </tr>
	<tr> <td>Math</td> <td>NaN</td> <td>name</td> <td>Number</td> <td>Object</td> </tr> 
	<tr> <td>prototype</td> <td>String</td> <td>toString</td> <td>undefined</td> <td>valueOf</td> </tr>
</table>


#Windows 保留关键字#

JavaScript 可以在 HTML 外部使用。它可在许多其他应用程序中作为编程语言使用。
在 HTML 中，您必须（为了可移植性，您也应该这么做）避免使用 HTML 和 Windows 对象和属性的名称作为 Javascript 的变量及函数名：
<table class="reference">
    <tr> <td>alert</td> <td>all</td> <td>anchor</td> <td>anchors</td> <td>area</td> </tr> 
    <tr> <td>assign</td> <td>blur</td> <td>button</td> <td>checkbox</td> <td>clearInterval</td> </tr> 
    <tr> <td>clearTimeout</td> <td>clientInformation</td> <td>close</td> <td>closed</td> <td>confirm</td> </tr> 
    <tr> <td>constructor</td> <td>crypto</td> <td>decodeURI</td> <td>decodeURIComponent</td> <td>defaultStatus</td> </tr> 
    <tr> <td>document</td> <td>element</td> <td>elements</td> <td>embed</td> <td>embeds</td> </tr> 
    <tr> <td>encodeURI</td> <td>encodeURIComponent</td> <td>escape</td> <td>event</td> <td>fileUpload</td> </tr> 
    <tr> <td>focus</td> <td>form</td> <td>forms</td> <td>frame</td> <td>innerHeight</td> </tr> 
    <tr> <td>innerWidth</td> <td>layer</td> <td>layers</td> <td>link</td> <td>location</td> </tr> 
    <tr> <td>mimeTypes</td> <td>navigate</td> <td>navigator</td> <td>frames</td> <td>frameRate</td> </tr> 
    <tr> <td>hidden</td> <td>history</td> <td>image</td> <td>images</td> <td>offscreenBuffering</td> </tr> 
    <tr> <td>open</td> <td>opener</td> <td>option</td> <td>outerHeight</td> <td>outerWidth</td> </tr> 
    <tr> <td>packages</td> <td>pageXOffset</td> <td>pageYOffset</td> <td>parent</td> <td>parseFloat</td> </tr> 
    <tr> <td>parseInt</td> <td>password</td> <td>pkcs11</td> <td>plugin</td> <td>prompt</td> </tr> 
    <tr> <td>propertyIsEnum</td> <td>radio</td> <td>reset</td> <td>screenX</td> <td>screenY</td> </tr> 
    <tr> <td>scroll</td> <td>secure</td> <td>select</td> <td>self</td> <td>setInterval</td> </tr> 
    <tr> <td>setTimeout</td> <td>status</td> <td>submit</td> <td>taint</td> <td>text</td> </tr> 
    <tr> <td>textarea</td> <td>top</td> <td>unescape</td> <td>untaint</td> <td>window</td> </tr>
</table>



#非标准 JavaScript (建议：不要使用它)#

一个实例是 const 关键字，用于定义变量。

一些 JavaScript 引擎把 const 当作 var 的同义词。另一些引擎则把 const 当作只读变量的定义。



#JavaScript JSON#

<table class="reference">
	<tr><th>函数</th><th>描述</th></tr> <tr><td><a target="_blank" href="http://www.runoob.com/js/javascript-json-parse.html">JSON.parse()</a></td><td>用于将一个 JSON 字符串转换为 JavaScript 对象。</td> </tr>
	<tr><td><a target="_blank" href="http://www.runoob.com/js/javascript-json-stringify.html">JSON.stringify()</a></td><td>用于将 JavaScript 值转换为 JSON 字符串。</td> </tr>
</table>



#JavaScript 函数#

函数可以通过声明定义，也可以是一个表达式。
>     function myFunction(a, b) {
>        return a * b;
>     }
>     
> ###
> 
> 函数表达式是匿名函数，通过变量名调用

>     var x = function (a, b) {return a * b}; 

> ###
> 
> 函数同样可以通过内置的 JavaScript 函数构造器（Function()）定义。

>     var myFunction = new Function("a", "b", "return a * b");

函数提升（Hoisting）-> 使用表达式定义函数时无法提升。

>     //函数可以在声明之前调用：
>     myFunction(5);
>     function myFunction(y) {
>         return y * y;
>     }

自调用函数

>     (function () {
>         var x = "Hello!!";  // 我将调用自己
>     })(); 


#JavaScript 函数参数#

函数显式参数 与 隐藏参数(arguments)

如果函数在调用时缺少参数，参数会默认设置为：undefined，但是建议最好为参数设置一个默认值： 
>     function myFunction(x, y) {
>         y = y || 0;
>     } 

###通过值传递参数###

> 
> 在函数中调用的参数是函数的参数。
> 
> 如果函数修改参数的值，将不会修改参数的初始值（在函数外定义）。
> 
> 函数参数的改变不会影响函数外部的变量（局部变量）。

###通过对象传递参数###

> 在JavaScript中，可以引用对象的值。
> 
> 因此我们在函数内部修改对象的属性就会修改其初始的值。
> 
> 修改对象属性可作用于函数外部（全局变量）。



#JavaScript 函数调用#

###this 关键字###

一般而言，在Javascript中，this指向函数执行时的当前对象。

函数不属于任何对象。但是在 JavaScript 中它始终是默认的全局对象(window)。

**当函数没有被自身的对象调用时， this 的值就会变成全局对象。**

**函数作为对象方法调用，会使得 this 的值成为对象本身。**





#作为函数方法调用函数#

> call() 和 apply() 是预定义的函数方法。 两个方法可用于调用函数，两个方法的第一个参数必须是对象本身。
>  
> 两者的区别在于第二个参数： apply传入的是一个参数数组，也就是将多个参数组合成为一个数组传入，而call则作为call的参数传入（从第二个参数开始）。 

 在 JavaScript 严格模式(strict mode)下, 在调用函数时第一个参数会成为 this 的值， 即使该参数不是一个对象。

在 JavaScript 非严格模式(non-strict mode)下, 如果第一个参数的值是 null 或 undefined, 它将使用全局对象替代。 

> 通过 call() 或 apply() 方法你可以设置 this 的值, 且作为已存在对象的新方法调用。


#JavaScript 闭包#

    var add = (function () {
    	var counter = 0;
    	return function () {return counter += 1;}
    })(); //自调用
    
    add();
    add();
    // 计数器为 2


> **JavaScript 闭包使得函数拥有私有变量变成可能。**
> 
> 计数器受匿名函数的作用域保护，只能通过 add 方法修改。
> 
> 闭包是可访问上一层函数作用域里变量的函数，即便上一层函数已经关闭。 


#JavaScript HTML DOM#

###查找 HTML 元素###

> 通过 id 查找 HTML 元素
> 
>     var x=document.getElementById("intro");
> 通过标签名查找 HTML 元素
> 
>     var x=document.getElementById("main");
>     var y=x.getElementsByTagName("p"); 

> 通过类名找到 HTML 元素
> 
>     //查找 class="intro" 的元素：
>     var x=document.getElementsByClassName("intro"); 

###JavaScript HTML DOM EventListener###

> 语法：element.addEventListener(event, function, useCapture);

>     该方法可以指定 "useCapture" 参数来设置传递类型：
>     默认值为 false, 即冒泡传递，当值为 true 时, 事件使用捕获传递。
>     
> ### 
> 
>     可以向同个元素添加多个同类型的事件
>     可以向同个元素添加不同类型的事件
>     
> ###
> 
>     removeEventListener() 方法移除由 addEventListener() 方法添加的事件句柄:
>     element.removeEventListener("mousemove", myFunction);

> **注意**： IE 8 及更早 IE 版本，Opera 7.0及其更早版本不支持 addEventListener() 和 removeEventListener() 方法。
> 但是，对于这类浏览器版本可以使用 detachEvent() 方法来移除事件句柄:

>     element.attachEvent(event, function);
>     element.detachEvent(event, function);


#JavaScript HTML DOM 元素(节点)#
    
    //添加元素
	var para=document.createElement("p");
    var node=document.createTextNode("这是一个新段落。");
    para.appendChild(node);
    
    var element=document.getElementById("div1");
    element.appendChild(para);

----------

    //删除元素
    var parent=document.getElementById("div1");
    var child=document.getElementById("p1");
    parent.removeChild(child); 


> 
> 如果能够在不引用父元素的情况下删除某个元素，就太好了。
> 不过很遗憾。DOM 需要清楚您需要删除的元素，以及它的父元素。
>
> 这是常用的解决方案：找到您希望删除的子元素，然后使用其 parentNode 属性来找到父元素：
> 
>     var child=document.getElementById("p1");
>     child.parentNode.removeChild(child);


#JavaScript 对象#

###JavaScript 中的所有事物都是对象：字符串、数值、数组、函数... ###

创建 JavaScript 对象

    person = new Object();
    person.firstname = "John";
    person.lastname  = "Doe";
    
替代语法（使用对象 literals）：

    person={firstname:"John", lastname:"Doe"}; 

对象构造器创建对象：

    function person(firstname,lastname,age,eyecolor)
    {
    	this.firstname = firstname;
    	this.lastname  = lastname;
    }
    var myFather=new person("John","Doe");
    


### JavaScript 类 ###

> JavaScript 是面向对象的语言，但 JavaScript 不使用类。
> 
> 在 JavaScript 中，不会创建类，也不会通过类来创建对象（就像在其他面向对象的语言中那样）。
>
> JavaScript 基于 prototype，而不是基于类的。


#JavaScript Number 对象#

> ###NaN不等于任何值，只能用函数 isNaN（）判断###
> ###Infinity与其他值的运算结果为Infinity或者NaN###

#JavaScript Window - 浏览器对象模型#

###Window 对象###

> 所有浏览器都支持 window 对象。它表示浏览器窗口。
>
> 所有 JavaScript 全局对象、函数以及变量均自动成为 window 对象的成员。
> 
> 全局变量是 window 对象的属性。
> 
> 全局函数是 window 对象的方法。
> 
> 甚至 HTML DOM 的 document 也是 window 对象的属性之一：

>      window.document.getElementById("header");
> 同
>
>      document.getElementById("header");

###Window 尺寸###

有三种方法能够确定浏览器窗口的尺寸（浏览器的视口，不包括工具栏和滚动条）。

对于Internet Explorer、Chrome、Firefox、Opera 以及 Safari：

    window.innerHeight - 浏览器窗口的内部高度
    window.innerWidth - 浏览器窗口的内部宽度

对于 Internet Explorer 8、7、6、5：

    document.documentElement.clientHeight
    document.documentElement.clientWidth

或者

    document.body.clientHeight
    document.body.clientWidth

实用的 JavaScript 方案（涵盖所有浏览器）：

    var w=window.innerWidth || document.documentElement.clientWidth || document.body.clientWidth;
    var h=window.innerHeight || document.documentElement.clientHeight || document.body.clientHeight;
> ###     

### Window 对象集合 ###
<table class="dataintable">
	<tr><th>集合</th><th>描述</th></tr>
	<tr>
		<td class="no_wrap">frames[]</td>
	    <td>
			<p>返回窗口中所有命名的框架。</p>
			<p>该集合是 Window 对象的数组，每个 Window 对象在窗口中含有一个框架或 &lt;iframe&gt;。属性 frames.length 存放数组 frames[] 中含有的元素个数。注意，frames[] 数组中引用的框架可能还包括框架，它们自己也具有 frames[] 数组。</p>
		</td>
	</tr>
</table>

### Window 对象属性 ###

<table class="dataintable">
	<tr>
		<th style="width:25%">属性</th><th>描述</th>
	</tr>
	<tr> 
		<td><a target="_blank" href="http://www.w3school.com.cn/jsref/prop_win_closed.asp">closed</a></td><td>返回窗口是否已被关闭。</td>  
	</tr>
	<tr>
		<td><a target="_blank" href="http://www.w3school.com.cn/jsref/prop_win_defaultstatus.asp">defaultStatus</a></td><td>设置或返回窗口状态栏中的默认文本。</td>
	</tr>
	<tr>
		<td><a target="_blank" href="http://www.w3school.com.cn/jsref/dom_obj_document.asp">document</a></td><td>对 Document 对象的只读引用。请参阅 <a target="_blank" href="dom_obj_document.asp">Document 对象</a>。</td>
	</tr>
	<tr>
		<td><a target="_blank" href="http://www.w3school.com.cn/jsref/dom_obj_history.asp">history</a></td><td>对 History 对象的只读引用。请参数 <a target="_blank" href="dom_obj_history.asp">History 对象</a>。</td>
	</tr>
	<tr>
		<td><a target="_blank" href="http://www.w3school.com.cn/jsref/prop_win_innerheight_innerwidth.asp">innerheight</a></td><td>返回窗口的文档显示区的高度。</td>
	</tr>
	<tr>
		<td><a target="_blank" href="http://www.w3school.com.cn/jsref/prop_win_innerheight_innerwidth.asp">innerwidth</a></td><td>返回窗口的文档显示区的宽度。</td>
	</tr>
	<tr><td>length</td><td>设置或返回窗口中的框架数量。</td></tr>
	<tr>
		<td><a target="_blank" href="http://www.w3school.com.cn/jsref/dom_obj_location.asp">location</a></td><td>用于窗口或框架的 Location 对象。请参阅 <a target="_blank" href="dom_obj_location.asp">Location 对象</a>。</td>
	</tr>
	<tr><td><a target="_blank" href="http://www.w3school.com.cn/jsref/prop_win_name.asp">name</a></td><td>设置或返回窗口的名称。</td></tr>
	<tr>
		<td><a target="_blank" href="http://www.w3school.com.cn/jsref/dom_obj_navigator.asp">Navigator</a></td><td>对 Navigator 对象的只读引用。请参数 <a target="_blank" href="http://www.w3school.com.cn/jsref/dom_obj_navigator.asp">Navigator 对象</a>。</td>
	</tr>
	<tr><td><a target="_blank" href="http://www.w3school.com.cn/jsref/prop_win_opener.asp">opener</a></td><td>返回对创建此窗口的窗口的引用。</td></tr>
	<tr><td><a target="_blank" href="http://www.w3school.com.cn/jsref/prop_win_outerheight.asp">outerheight</a></td> <td>返回窗口的外部高度。</td>  </tr>
	<tr> <td><a target="_blank" href="http://www.w3school.com.cn/jsref/prop_win_outerwidth.asp">outerwidth</a></td> <td>返回窗口的外部宽度。</td> </tr>
	<tr> <td>pageXOffset</td> <td>设置或返回当前页面相对于窗口显示区左上角的 X 位置。</td> </tr>
	<tr> <td>pageYOffset</td> <td>设置或返回当前页面相对于窗口显示区左上角的 Y 位置。</td> </tr>
	<tr> <td>parent</td> <td>返回父窗口。</td></tr>
	<tr><td><a target="_blank" href="http://www.w3school.com.cn/jsref/dom_obj_screen.asp">Screen</a></td><td>对 Screen 对象的只读引用。请参数 <a target="_blank" href="http://www.w3school.com.cn/jsref/dom_obj_screen.asp">Screen 对象</a>。</td></tr>
	<tr><td><a target="_blank" href="http://www.w3school.com.cn/jsref/prop_win_self.asp">self</a></td><td>返回对当前窗口的引用。等价于 Window 属性。</td></tr>
	<tr><td><a target="_blank" href="http://www.w3school.com.cn/jsref/prop_win_status.asp">status</a></td><td>设置窗口状态栏的文本。</td></tr>
	<tr>
		<td><a target="_blank" href="http://www.w3school.com.cn/jsref/prop_win_top.asp">top</a></td><td>返回最顶层的先辈窗口。</td>
	</tr>
	<tr>
		<td>window</td><td>window 属性等价于 self 属性，它包含了对窗口自身的引用。</td>
	</tr>
	<tr>
		<td>
			<ul>
				<li>screenLeft</li>
				<li>screenTop</li>
				<li>screenX</li>
				<li>screenY</li>
			</ul>
		</td>
		<td>只读整数。声明了窗口的左上角在屏幕上的的 x 坐标和 y 坐标。IE、Safari 和 Opera 支持 screenLeft 和 screenTop，而 Firefox 和 Safari 支持 screenX 和 screenY。</td>
	</tr>
</table>


# Window 对象方法 #

<table class="dataintable">
  <tbody><tr>
    <th style="width:25%">方法</th>
    <th>描述</th>
  </tr>
  <tr>
    <td><a target="_blank" href="http://www.w3school.com.cn/jsref/met_win_alert.asp">alert()</a></td>
    <td>显示带有一段消息和一个确认按钮的警告框。</td>
  </tr>
  <tr>
    <td><a target="_blank" href="http://www.w3school.com.cn/jsref/met_win_blur.asp">blur()</a></td>
    <td>把键盘焦点从顶层窗口移开。</td>
  </tr>
  <tr>
    <td><a target="_blank" href="http://www.w3school.com.cn/jsref/met_win_clearinterval.asp">clearInterval()</a></td>
    <td>取消由 setInterval() 设置的 timeout。</td>
  </tr>
  <tr>
    <td><a target="_blank" href="http://www.w3school.com.cn/jsref/met_win_cleartimeout.asp">clearTimeout()</a></td>
    <td>取消由 setTimeout() 方法设置的 timeout。</td>
  </tr>
  <tr>
    <td><a target="_blank" href="http://www.w3school.com.cn/jsref/met_win_close.asp">close()</a></td>
    <td>关闭浏览器窗口。</td>
  </tr>
  <tr>
    <td><a target="_blank" href="http://www.w3school.com.cn/jsref/met_win_confirm.asp">confirm()</a></td>
    <td>显示带有一段消息以及确认按钮和取消按钮的对话框。</td>
  </tr>
  <tr>
    <td><a target="_blank" href="http://www.w3school.com.cn/jsref/met_win_createpopup.asp">createPopup()</a></td>
    <td>创建一个 pop-up 窗口。</td>
  </tr>
  <tr>
    <td><a target="_blank" href="http://www.w3school.com.cn/jsref/met_win_focus.asp">focus()</a></td>
    <td>把键盘焦点给予一个窗口。</td>
  </tr>
  <tr>
    <td><a target="_blank" href="http://www.w3school.com.cn/jsref/met_win_moveby.asp">moveBy()</a></td>
    <td>可相对窗口的当前坐标把它移动指定的像素。</td>
  </tr>
  <tr>
    <td><a target="_blank" href="http://www.w3school.com.cn/jsref/met_win_moveto.asp">moveTo()</a></td>
    <td>把窗口的左上角移动到一个指定的坐标。</td>
  </tr>
  <tr>
    <td><a target="_blank" href="http://www.w3school.com.cn/jsref/met_win_open.asp">open()</a></td>
    <td>打开一个新的浏览器窗口或查找一个已命名的窗口。</td>
  </tr>
  <tr>
    <td><a target="_blank" href="http://www.w3school.com.cn/jsref/met_win_print.asp">print()</a></td>
    <td>打印当前窗口的内容。</td>
  </tr>
  <tr>
    <td><a target="_blank" href="http://www.w3school.com.cn/jsref/met_win_prompt.asp">prompt()</a></td>
    <td>显示可提示用户输入的对话框。</td>
  </tr>
  <tr>
    <td><a target="_blank" href="http://www.w3school.com.cn/jsref/met_win_resizeby.asp">resizeBy()</a></td>
    <td>按照指定的像素调整窗口的大小。</td>
  </tr>
  <tr>
    <td><a target="_blank" href="http://www.w3school.com.cn/jsref/met_win_resizeto.asp">resizeTo()</a></td>
    <td>把窗口的大小调整到指定的宽度和高度。</td>
  </tr>
  <tr>
    <td><a target="_blank" href="http://www.w3school.com.cn/jsref/met_win_scrollby.asp">scrollBy()</a></td>
    <td>按照指定的像素值来滚动内容。</td>
  </tr>
  <tr>
    <td><a target="_blank" href="http://www.w3school.com.cn/jsref/met_win_scrollto.asp">scrollTo()</a></td>
    <td>把内容滚动到指定的坐标。</td>
  </tr>
  <tr>
    <td><a target="_blank" href="http://www.w3school.com.cn/jsref/met_win_setinterval.asp">setInterval()</a></td>
    <td>按照指定的周期（以毫秒计）来调用函数或计算表达式。</td>
  </tr>
  <tr>
    <td><a target="_blank" href="http://www.w3school.com.cn/jsref/met_win_settimeout.asp">setTimeout()</a></td>
    <td>在指定的毫秒数后调用函数或计算表达式。</td>
  </tr>
</tbody></table>

#Window Screen#
> screen.availWidth 属性返回访问者屏幕的宽度，以像素计，减去界面特性，比如窗口任务栏。
> 
    screen.availWidth - 可用的屏幕宽度
    screen.availHeight - 可用的屏幕高度


#Window Location #

    location.hostname 返回 web 主机的域名
    location.pathname 返回当前页面的路径和文件名
    location.port 返回 web 主机的端口 （80 或 443）
    location.protocol 返回所使用的 web 协议（http:// 或 https://）



# Window History #
> 为了保护用户隐私，对 JavaScript 访问该对象的方法做出了限制。

    history.back() - 与在浏览器点击后退按钮相同
    history.forward() - 与在浏览器中点击按钮向前相同

# Navigator 对象 #

<table class="dataintable">
	<tr>
		<th style="width:30%">集合</th><th>描述</th>
	</tr>
    <tr>
		<td class="no_wrap">plugins[]</td><td><p>返回对文档中所有嵌入式对象的引用。</p>
	<p>该集合是一个 Plugin 对象的数组，其中的元素代表浏览器已经安装的插件。Plug-in 对象提供的是有关插件的信息，其中包括它所支持的 MIME 类型的列表。</p>
	<p>虽然 plugins[] 数组是由 IE 4 定义的，但是在 IE 4 中它却总是空的，因为 IE 4 不支持插件和 Plugin 对象。</p></td>
	</tr>
</table>

###Navigator 对象属性###

<table class="dataintable">
	<tr><th style="width:30%">属性</th><th>描述</th></tr>
	<tr><td><a target="_blank" href="http://www.w3school.com.cn/jsref/prop_nav_appcodename.asp">appCodeName</a></td><td>返回浏览器的代码名。</td></tr>
	<tr><td><a target="_blank" href="http://www.w3school.com.cn/jsref/prop_nav_appminorversion.asp">appMinorVersion</a></td><td>返回浏览器的次级版本。</td>	</tr>
	<tr><td><a target="_blank" href="http://www.w3school.com.cn/jsref/prop_nav_appname.asp">appName</a></td><td>返回浏览器的名称。</td></tr>
	<tr><td><a target="_blank" href="http://www.w3school.com.cn/jsref/prop_nav_appversion.asp">appVersion</a></td><td>返回浏览器的平台和版本信息。</td></tr>
	<tr><td><a target="_blank" href="http://www.w3school.com.cn/jsref/prop_nav_browserlanguage.asp">browserLanguage</a></td><td>返回当前浏览器的语言。</td>	</tr>
	<tr><td><a target="_blank" href="http://www.w3school.com.cn/jsref/prop_nav_cookieenabled.asp">cookieEnabled</a></td><td>返回指明浏览器中是否启用 cookie 的布尔值。</td></tr>
	<tr><td><a target="_blank" href="http://www.w3school.com.cn/jsref/prop_nav_cpuclass.asp">cpuClass</a></td><td>返回浏览器系统的 CPU 等级。</td></tr>
	<tr><td><a target="_blank" href="http://www.w3school.com.cn/jsref/prop_nav_online.asp">onLine</a></td><td>返回指明系统是否处于脱机模式的布尔值。</td>	</tr>
	<tr><td><a target="_blank" href="http://www.w3school.com.cn/jsref/prop_nav_platform.asp">platform</a></td><td>返回运行浏览器的操作系统平台。</td></tr>
	<tr>
		<td><a target="_blank" href="http://www.w3school.com.cn/jsref/prop_nav_systemlanguage.asp">systemLanguage</a></td>
		<td>返回 OS 使用的默认语言。</td>
	</tr>
	<tr>
		<td><a target="_blank" href="http://www.w3school.com.cn/jsref/prop_nav_useragent.asp">userAgent</a></td>
		<td>返回由客户机发送服务器的 user-agent 头部的值。</td>
	</tr>
	<tr>
		<td><a target="_blank" href="http://www.w3school.com.cn/jsref/prop_nav_userlanguage.asp">userLanguage</a></td>
		<td>返回 OS 的自然语言设置。</td>
	</tr>
</table>

#JavaScript 计时事件#


    setInterval() - 间隔指定的毫秒数不停地执行指定的代码。
	clearInterval() 方法用于停止 setInterval() 方法执行的函数代码。
	
    setTimeout() - 暂停指定的毫秒数后执行指定的代码
	clearTimeout() 方法用于停止执行setTimeout()方法的函数代码。


#JavaScript Cookies#

###使用 JavaScript 创建(或修改) Cookie###

JavaScript 可以使用 document.cookie 属性来创建 、读取、及删除 cookies。

JavaScript 中，创建 cookie 如下所示：

     document.cookie="username=John Doe";

您还可以为 cookie 添加一个过期时间（以 UTC 或 GMT 时间）。默认情况下，cookie 在浏览器关闭时删除：

     document.cookie="username=John Doe; expires=Thu, 18 Dec 2013 12:00:00 GMT";

您可以使用 path 参数告诉浏览器 cookie 的路径。默认情况下，cookie 属于当前页面。

    document.cookie="username=John Doe; expires=Thu, 18 Dec 2013 12:00:00 GMT; path=/";

### 使用 JavaScript 删除 Cookie ###

删除 cookie 非常简单。您只需要设置 expires 参数为以前的时间即可，如下所示，设置为 Thu, 01 Jan 1970 00:00:00 GMT:

	document.cookie = "username=; expires=Thu, 01 Jan 1970 00:00:00 GMT";

**注意，当您删除时不必指定 cookie 的值。**

    function setCookie(cname,cvalue,exdays)
    {
	    var d = new Date();
	    d.setTime(d.getTime()+(exdays*24*60*60*1000));
	    var expires = "expires="+d.toGMTString();
	    document.cookie = cname + "=" + cvalue + "; " + expires;
    }
    
    function getCookie(cname)
    {
	    var name = cname + "=";
	    var ca = document.cookie.split(';');
	    for(var i=0; i<ca.length; i++)
	    {
	        var c = ca[i].trim();
	        if (c.indexOf(name)==0) return c.substring(name.length,c.length);
	    }
	    return "";
    }
    
    function checkCookie()
    {
	    var user=getCookie("username");
	    if (user!=""){
	        alert("Welcome again " + user);
	    }else{
	        user = prompt("Please enter your name:","");
	        if (user!="" && user!=null){
	            setCookie("username",user,365);
	        }
	    }
    }