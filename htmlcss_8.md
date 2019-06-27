
# 72  css属性font-style用于设置字体的粗细。请判断这句话的正确与否

>        答案:false
>        解释：
>            font-style是设置字体的风格，包括值normal：默认正常情况；italic：显示文字为斜体；oblique：显示文字为斜体；inherit：从父亲那继承一个样式字体；
>            font-weight为设置字体的粗细。
>            font-style设置字体样式  
>            normal:正常字体
>            italic:显示文字为斜体（该字体有斜体样式时使用）
>            oblique:显示文字为斜体（该字体没有斜体样式时使用，文字斜体显示）
>            inherit:从父亲哪里继承样式
>            font-weight:改变文字粗细  属性值有normal  bold 100~900 inherit

# 73  对于下拉菜单，错误的是

        <div class="dropdown">
        <button class="btn btn-default dropdown-toggle" type="button" id="dropdownMenu1" data-toggle="dropdown">
        Dropdown
        <span class="caret"></span>
        </button>
        <ul class="dropdown-menu" role="menu" aria-labelledby="dropdownMenu1">
        <li role="presentation"><a role="menuitem" tabindex="-1" href="#">Action</a></li>
        <li role="presentation"><a role="menuitem" tabindex="-1" href="#">Another action</a></li>
        <li role="presentation"><a role="menuitem" tabindex="-1" href="#">Something else here</a></li>
        <li role="presentation"><a role="menuitem" tabindex="-1" href="#">Separated link</a></li>
        </ul>
        </div>
            A    表示了一个有五个下拉选项的下拉菜单
            B    <span class="caret"></span>可以去掉而不影响功能
            C    可以加入pull-right使菜单右对齐
            D    可加入dropdown-menu-right使菜单右对齐

>        答案: A 
>        解释：
>            通过向 .dropdown-menu 添加 .pull-right 类来向右对齐下拉菜单。 
>            Bootstrap默认情况下，下拉菜单自动沿着父元素的上沿和左侧被定位为 100% 宽度。 为 .dropdown-menu 添加 .dropdown-menu-right 类可以让菜单右对齐。

# 74  下面有关CSS中link和@import的区别，描述错误的是？

            A    link属于XHTML标签，而@import完全是CSS提供的一种方式
            B    当一个页面被加载的时候，link引用的CSS会同时被加载，而@import引用的CSS会等到页面全部被下载完再被加载
            C    link在支持CSS的浏览器上都支持而@import只在5.0以上的版本有效
            D    当使用javascript控制dom去改变样式的时候，只能使用@import方式

>        答案: D 
>        解释： 
>            1，@import url（）机制是不同于link的，link是在加载页面前把css加载完毕，而@import url（）则是读取完文件后在加载，所以会出现一开始没有css样式，闪烁一下出现样式后的页面(网速慢的情况下)。  
>            2，@import 是css2里面的，所以古老的ie5不支持。  
>            3，当使用javascript控制dom去改变样式的时候，只能使用link标签，因为@import不是dom可以控制的。
>            4，link除了能加载css外还能定义RSS，定义rel连接属性，@import只能加载css  

# 75  下面哪个属性不会让 div 脱离文档流（normal flow）

            A    position: absolute;
            B    position: fixed;
            C    position: relative;
            D    float: left;

>        答案: C  
>        解释：
>            A：position: absolute;生成绝对定位的元素，相对于static 定位以外的第一个父元素进行定位；都绝对定位了，肯定脱离了文档流。。
>            B:position: fixed;生成绝对定位的元素，相对于浏览器窗口进行定位;相对于浏览器了，也和正常顺序排下来没什么关系。。
>            C:position: relative;生成相对定位的元素，相对于其正常位置进行定位。生成相对定位，也就是说还在原本的上下左右之间，上下左右的元素都不变，so这个没有能脱离文档流。。就这个了
>            D:float: left;都浮动出去了，还上哪保持原位置去。最终答案选择C

# 76  有一段html代码：

    <div style=”color:red; text-color:blue;”><span   style=”color:green;text-color:black;”>Hello</span></div>,
    那么”Hello”的字体颜色是（）
            A    red
            B    blue
            C    green
            D    black

>        答案: C
>        解释：
>            没有text-color这个属性，文字颜色统一用color.再加上就近原则

# 77  在实际使用中，下面哪一个可以很方便的获得页面中定义的HTML对象？（）

            A    document.GetElementsByTagName
            B    document.getElementByTagNames
            C    document.getElementsById
            D    document.getElementById

>        答案: D
>        解释：
>            A错在首字母大写，应为get……，后面是对的； B错在s，正确应为getElementsByTagName； C也错在s，正确应为getElementById； 记住首字母小写，Id无s，TageName有s就好了

# 78  有一个元素，需要在pc端显示而在手机端隐藏，需要使用的方法是？

            A    visible-xs-8 hidden-md
            B    visible-md-8 hidden-xs
            C    visible-md-8 hidden-sm
            D    visible-sm-8 hidden-md

>        答案: B
>        解释：
>            bootstrap3.x使用了四种栅格选项来形成栅格系统，这里跟大家详解一下
>            四种栅格选项之间的区别， 其实区别只有一条就是适合不同尺寸的屏幕设备 。
>            我们看class前缀这一项，我们姑且以前缀命名这四种栅格选项，
>            他们分别是col-xs、col-sm、col-md、col-lg，我们懂英文的就知道，
>            lg是large的缩写，md是mid的缩写，sm是small的缩写，
>            xs是extremely small的缩写。
>            mobile – xs ( <768px )
>            tablet – sm ( 768~991px )
>            desktop – md ( 992~1170px )
>            large desktop – lg ( >1170px )

# 79  获取 input 节点的正确方法是(  )

        <form class="file" name="upload">
        <input id="file" name="file" />
        </form>
            A    document.querySelectorAll('file')[0]
            B    document.getElementById('file')[0]
            C    document.getElementByTagName('file')[0]
            D    document.getElementsByClassName('file')[0]

>        答案: D  
>        解释：
>            document.querySelectorALL() 方法返回匹配的元素集合，如果没有匹配项，返回空的nodelist(节点数组) 
>            该方法接受三种类型的参数：id(#)，class(.)，标签  
>            所以A选项应该改为
>            document.querySelectorAll('.file')[0]
>            getElementById() 方法是返回对拥有指定 ID 的第一个对象的引用 并不是一个数组
>            getElementByTagName()返回带有指定标签名的对象集合 file不是标签名_(:з」∠)_
>            getElementSByClassName()返回特定类名的对象集合（IE8好像不适用

# 80  现有如下html结构

        <ul>
        <li>click me</li>
        <li>click me</li>
        <li>click me</li>
        <li>click me</li>
        </ul>
        运行如下代码：
            var elements=document.getElementsByTagName('li');
            var length=elements.length;
            for(var i=0;i<length;i++){
                elements[i].onclick=function(){
                alert(i);
            }
        }
        依次点击4个li标签，哪一个选项是正确的运行结果（）?
            A    依次弹出1，2，3，4
            B    依次弹出0，1，2，3
            C    依次弹出3，3，3，3
            D    依次弹出4，4，4，4

>        答案: D  
>        解释：
>            因点击为匿名函数，其执行到这里的时候 i 已是 4，即不会改变~
>            这里考的是JS的运行机制！ 事件(click,focus等等)，定时器(setTimeout和setInterval)，
>            ajax,都是会触发异步，属于异步任务；js是单线程的，一个时间点只能做一件事，优先处理同步任务；
>            按照代码从上往下执行，遇到异步，就挂起，放到异步任务里，继续执行同步任务，只有同步任务执行完了，
>            才去看看有没有异步任务，然后再按照顺序执行！ 这里for循环是同步任务，onclick是异步任务，所以等for循环执行完了
>            ，i变成4了，注意：这里因为i是全局变量，最后一个i++，使得i为4(后面的onclick函数，最后在循环外面执行
>            ，不受i<length限制)； 所以for循环每执行一次，onclick事件函数都会被挂起一次，共4次； for循环结束后
>            ，点击事件 触发了4个onclick函数，接着输出4个4！ 
