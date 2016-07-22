##两大要点  

###1、通过DOM即document全局对象获取元素并操作之

	document.getElementById(id).innerHTML=new HTML
	document.getElementById(id).style.property=new style
	var para=document.createElement("p");
	var node=document.createTextNode("这是新段落。");
	para.appendChild(node);


###2、通过设置事件和响应函数实现动态页面

显式设置函数

	<!DOCTYPE html>
	<html>
	<head>
	<script>
	function changetext(id)
	{
	id.innerHTML="谢谢!";
	}
	</script>
	</head>
	<body>

	<h1 onclick="changetext(this)">请点击该文本</h1>

	</body>
	</html>

隐式设置函数

	<!DOCTYPE html>
	<html>
	<body>

	<h1 onclick="this.innerHTML='谢谢!'">请点击该文本</h1>

	</body>
	</html>


##Javascript内置对象
javascript一切皆对象，除原始值外，函数也是对象哟（类似于C++中的函数指针）  
原始值 vs 对象  
javascript 中的值可以被划分为两大类：原始值（primitive）和对象（object）。  
定义  
javascript 的两种值的定义：  
下面的值是原始值。  
1.字符串  
2.数字：在 JavaScript 中所有的数字都是浮点数  
3.布尔值  
4.null  
5.undefined  
  
所有其它的值都是对象（object）。对象可以进一步划分：  
内置全局对象是Javascirpt编程的基石，例如：document、String、function等  
###1、JavaScript 对象  
JS Array  
JS Boolean  
JS Date  
JS Math  
JS Number  
JS String  
JS RegExp  
JS Functions  
JS Events  
###2、Browser 对象  
Window  
Navigator  
Screen  
History  
Location  
###3、HTML DOM 对象  
DOM Document  
DOM Element  
DOM Attribute  
DOM Event  
###4、HTML 对象  
<a>  
<area>  
<audio>  
<base>  
<body>  
<blockquote>  
<button>  
<canvas>  
<col>  
<colgroup>  
<datalist>  
<del>  
<details>  
<dialog>  
<embed>  
<fieldset>  
<form>  
<frame>  
<frameset>  
<iframe>  
<img>  
<ins>  
<input> button  
<input> checkbox  
<input> color  
<input> date  
<input> datetime  
<input> datetime-local  
<input> email  
<input> file  
<input> hidden  
<input> image  
<input> month  
<input> number  
<input> password  
<input> range  
<input> radio  
<input> reset  
<input> search  
<input> submit  
<input> text  
<input> time  
<input> url  
<input> week  
<keygen>  
<label>  
<legend>  
<li>  
<link>  
<map>  
<menu>  
<menuitem>  
<meta>  
<meter>  
<object>  
<ol>  
<optgroup>  
<option>  
<param>  
<progress>  
<q>  
<script>  
<select>  
<source>  
<style>  
<table>  
<td>  
<th>  
<tr>  
<textarea>  
<time>  
<title>  
<track>  
<video>  