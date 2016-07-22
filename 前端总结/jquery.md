##一、JQUERY简介
jQuery 是一个 JavaScript 函数库。 
jQuery 库包含以下特性： 
HTML 元素选取  
HTML 元素操作  
CSS 操作   
HTML 事件函数   
JavaScript 特效和动画   
HTML DOM 遍历和修改  
AJAX   
Utilities  

##二、JQuery的安装
jQuery 库位于一个 JavaScript 文件中，其中包含了所有的 jQuery 函数。   
###1、可以通过下面的标记把 jQuery 添加到网页中：  

	<head>    
	<script type="text/javascript" src="jquery.js"></script>    
	</head>    

###2、库的替代
Google 和 Microsoft 对 jQuery 的支持都很好。   
如果您不愿意在自己的计算机上存放 jQuery 库，那么可以从 Google 或 Microsoft 加载 CDN jQuery 核心文件。   
使用 Google 的 CDN   

	<head>   
	<script type="text/javascript" src="http://ajax.googleapis.com/ajax/libs   
	/jquery/1.4.0/jquery.min.js"></script>  
	</head>   

使用 Microsoft 的 CDN   

	<head>   
	<script type="text/javascript" src="http://ajax.microsoft.com/ajax/jquery   
	/jquery-1.4.min.js"></script>   
	</head>   

##三、基本语法介绍
###1、jQuery 语法  
jQuery 语法是为 HTML 元素的选取编制的，可以对元素执行某些操作。  
*基础语法是：$(selector).action()* 
1、美元符号定义 jQuery  
2、选择符（selector）“查询”和“查找” HTML 元素  
3、jQuery 的 action() 执行对元素的操作  

*示例*  
1、$(this).hide() - 隐藏当前元素  this当前元素选择器
2、$("p").hide() - 隐藏所有段落  标签选择器   
3、$(".test").hide() - 隐藏所有 class="test" 的所有元素  class选择器  
4、$("#test").hide() - 隐藏所有 id="test" 的元素  id选择器   
提示：jQuery 使用的语法是 XPath 与 CSS 选择器语法的组合。在本教程接下来的章节，您将学习到更多有关选择器的语法。  

###2、jQuery 选择器
在前面的章节中，我们展示了一些有关如何选取 HTML 元素的实例。  
关键点是学习 jQuery 选择器是如何准确地选取您希望应用效果的元素。  
jQuery 元素选择器和属性选择器允许您通过标签名、属性名或内容对 HTML 元素进行选择。  
选择器允许您对 HTML 元素组或单个元素进行操作。  
在 HTML DOM 术语中：  
选择器允许您对 DOM 元素组或单个 DOM 节点进行操作。  
1、*jQuery 元素选择器*  
$("p") 选取 <p> 元素。  
$("p.intro") 选取所有 class="intro" 的 <p> 元素。  
$("p#demo") 选取所有 id="demo" 的 <p> 元素。  

2、*jQuery 使用 XPath 表达式来选择带有给定属性的元素*  
$("[href]") 选取所有带有 href 属性的元素。  
$("[href='#']") 选取所有带有 href 值等于 "#" 的元素。  
$("[href!='#']") 选取所有带有 href 值不等于 "#" 的元素。  
$("[href$='.jpg']") 选取所有 href 值以 ".jpg" 结尾的元素。 

3、*jQuery CSS 选择器*  
jQuery CSS 选择器可用于改变 HTML 元素的 CSS 属性。  
下面的例子把所有 p 元素的背景颜色更改为红色：  
实例  
$("p").css("background-color","red");  


###3、文档就绪函数
您也许已经注意到在我们的实例中的所有 jQuery 函数位于一个 document ready 函数中：  

	$(document).ready(function(){  
	  
	--- jQuery functions go here ----  
	  
	});  

这是为了*防止文档在完全加载（就绪）之前运行 jQuery代码*。  
如果在文档没有完全加载之前就运行函数，操作可能失败。下面是两个具体的例子：  
试图隐藏一个不存在的元素  
获得未完全加载的图像的大小  



###4、jQuery 事件函数
jQuery 是为事件处理特别设计的。  
1、jQuery 事件处理方法是 jQuery 中的核心函数。  
事件处理程序指的是当 HTML 中发生某些事件时所调用的方法。术语由事件“触发”（或“激发”）经常会被使用。  
通常会把 jQuery 代码放到 <head>部分的事件处理方法中：

2、jQuery 名称冲突  

jQuery 使用 $ 符号作为 jQuery 的简介方式。  
某些其他 JavaScript 库中的函数（比如 Prototype）同样使用 $ 符号。  
jQuery 使用名为 noConflict() 的方法来解决该问题。  
var jq=jQuery.noConflict()，帮助您使用自己的名称（比如 jq）来代替 $ 符号。  
亲自试一试  

3、结论  

	由于 jQuery 是为处理 HTML 事件而特别设计的，那么当您遵循以下原则时，您的代码会更恰当且更易维护：  
	把所有 jQuery 代码置于事件处理函数中  
	把所有事件处理函数置于文档就绪事件处理器中  
	把 jQuery 代码置于单独的 .js 文件中  
	如果存在名称冲突，则重命名 jQuery 库  


4、jQuery 事件  
下面是 jQuery 中事件方法的一些例子：  
Event 函数	绑定函数至  

	$(document).ready(function)	将函数绑定到文档的就绪事件（当文档完成加载时）  
	$(selector).click(function)	触发或将函数绑定到被选元素的点击事件  
	$(selector).dblclick(function)	触发或将函数绑定到被选元素的双击事件  
	$(selector).focus(function)	触发或将函数绑定到被选元素的获得焦点事件  
	$(selector).mouseover(function)	触发或将函数绑定到被选元素的鼠标悬停事件  
如需完整的参考手册，请访问我们的 jQuery 事件参考手册。  


##四、JQuery元素拾取与操作
###1、jQuery 语法元素拾取
$符号，美元号Dollar表示引用JQuery对HTML的DOM进行操作；操作可以包括择取、事件响应、样式改变等    
$(this).hide()  
演示 jQuery hide() 函数，隐藏当前的（以this作为选择参数） HTML 元素。  
$("#test").hide()  
演示 jQuery hide() 函数，隐藏 id="test" 的元素。  
$("p").hide()  
演示 jQuery hide() 函数，隐藏所有 <p> 元素。  
$(".test").hide()  
演示 jQuery hide() 函数，隐藏所有 class="test" 的元素。


###2、设置
1、设置内容 - text()、html() 以及 val()
text() - 设置或返回所选元素的文本内容
html() - 设置或返回所选元素的内容（包括 HTML 标记）
val() - 设置或返回表单字段的值

	$("#btn1").click(function(){
	  $("#test1").text("Hello world!");
	});
	$("#btn2").click(function(){
	  $("#test2").html("<b>Hello world!</b>");
	});
	$("#btn3").click(function(){
	  $("#test3").val("Dolly Duck");
	});

2、设置属性 - attr()
jQuery attr() 方法也用于设置/改变属性值。
下面的例子演示如何改变（设置）链接中 href 属性的值：
实例

	$("button").click(function(){
	  $("#w3s").attr("href","http://www.w3school.com.cn/jquery");
	});


3、jQuery - 删除元素
jQuery 添加  
jQuery CSS 类  
通过 jQuery，可以很容易地删除已有的 HTML 元素。  
删除元素/内容  
如需删除元素和内容，一般可使用以下两个 jQuery 方法：  
remove() - 删除被选元素（及其子元素）  
empty() - 从被选元素中删除子元素  
jQuery remove() 方法  
jQuery remove() 方法删除被选元素及其子元素。  

实例  

	$("#div1").remove();


4、通过 jQuery，可以很容易地添加新元素/内容。  
添加新的 HTML 内容  
我们将学习用于添加新内容的四个 jQuery 方法：  
append() - 在被选元素的结尾插入内容  
prepend() - 在被选元素的开头插入内容  
after() - 在被选元素之后插入内容  
before() - 在被选元素之前插入内容  
  



