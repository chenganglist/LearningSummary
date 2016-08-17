##prototype 属性允许您向对象添加属性和方法

注意： Prototype 是全局属性，适用于所有的Javascript对象。
语法

    object.prototype.name=value

浏览器支持
Internet ExplorerFirefoxOperaGoogle ChromeSafari
所有主要浏览器都支持 prototype 属性
实例
实例
适用 prototype 属性给对象添加属性:

    <script>

    function employee(name,jobtitle,born)
    {
        this.name=name;
        this.jobtitle=jobtitle;
        this.born=born;
    }

    var fred=new employee("Fred Flintstone","Caveman",1970);
    employee.prototype.salary=null;
    fred.salary=20000;

    document.write(fred.salary);

    </script>
    
以上实例输出结果:
20000