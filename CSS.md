# css
## css基础
css对块级元素和内联元素形成的盒子进行控制；<br/>
css通过<b>规则</b>与HTML元素想关联来工作；<br/>
css规则包括：选择器 和 声明;
<ul> <li>选择器，选择要应用规则的元素，多个元素用逗号隔开</li>
<li>声明，{属性1：值1 ； 属性2：值2；}</li>
</ul>
/*  */ css的注释语句<br/>
HTML文档使用外部CSS
<ul> <li>&ltlink&gt元素，寻找css文件；位于head元素中</li>
<li>href特性：css文件路径</li>
<li>type特性：文档类型text/css</li>
<li>rel特性：链接关系，css文件对应stylesheet</li>
<li>推荐使用</li>
</ul>
使用内部CSS
<UL>
<li>&LTstyle>元素，位于head元素中</li>
<li>type特性：文档类型text/css</li>
</ul>
CSS选择器
<table>
<tr><th scope="col">选择器</th>
    <th scope="col">含义</th>
    <th scope="col">示例</th>
</tr>
<tr>
    <td>通用选择器</td>
    <td>应用于所有元素</td>
    <td>*{ }</td>
</tr>
<tr>
    <td>类型选择器</td>
    <td>元素名称</td>
    <td>h1,h2,p,body{ }</td>
</tr>
<tr>
    <td>类选择器</td>
    <td>calss特性值</td>
    <td>.note{ } <br/> p.note{ } </td>
</tr>
<tr>
    <td>ID选择器</td>
    <td>元素ID的特性值</td>
    <td>#introduction{ }</td>
</tr>
<tr>
    <td>子元素选择器</td>
    <td>指定元素的直接子元素</td>
    <td>li>a{ }<br>
        父元素为li的a </td>
</tr>
<tr>
    <td>后代选择器</td>
    <td>后代元素</td>
    <td>p a{ }<br>
        p元素中的a，无论有无嵌套</td>
</tr>
<tr>
    <td>相邻兄弟选择器</td>
    <td>相邻的兄弟元素</td>
    <td>h1+p{ }<br>
        h1之后第一个p元素</td>
</tr>
<tr>
    <td>普通兄弟选择器</td>
    <td>兄弟元素</td>
    <td>h1~p{ }</td>
</tr>
</table>

CSS规则级联<br/>
<ol>
<li>就近原则，后出现优先于先出现</li>
<li>具体原则，描述具体的优先于一般选择器</li>
<li>重要性，！important</li>
</ol>

继承：padding：inherit，强制大所属元素从父元素继承属性值

## 颜色
<ul>
<li>前景色</li>
color属性指定文本的颜色；<br/>
三种方法指定颜色
<OL>
<li>RGB值</li>
    color：rgb（100，100，90）;
<li>十六进制编码</li>
    color：#ee3e80;
<li>颜色名称</li>
    color:darkcyan;
</ol>

<li>背景色</li>
background-color

<li>透明度</li>
opacity，属性值为0~1<br/>
rgba,中的a也可以设置透明度

<li>css3:HSL和HSLA</li>
色调、饱和度、明度、透明度<br/>
background-color:#ffffff;<br/>
background-color:hsla(0,100%,100%,0.5);
