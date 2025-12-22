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
</ul>

## 文本
<ul>
    <li>字体术语</li>
        <ul>
            <li>衬线字体</li>
            字母末端有装饰，便于阅读，用于长篇文本
            <li>无衬线字体</li>
            文本比较小时，便于阅读
            <li>等宽字体</li>
            便于文本的跟随，常用于显示代码
        </ul>
    <li>字体选用</li>
        <ul>
            <li>font-family</li>
            可以指定一组字体，以防止用户没有安装指定的字体<br/>
            eg： font-family：Arial, Verdana,"Courier New";<br/>
            多个单词组成的要用双引号。
        </ul>
    <li>字体大小</li>
         <ul>
            <li>font-size</li>
            - 像素<br/>
            eg： font-size：12px;<br/>
            - 百分比<br/>
            默认大小为16px<br/>
            eg：font-size:200%;<br/>
            - EM值<br/>
            1个em相当于1个字母m的宽度
        </ul>
    <li>选用更多的字体 @font-face {font-family， src}</li>
    <li>粗体</li>
        <ul>
            <li>font-weight</li>
                normal，bold，<br/>
        </ul>
    <li>斜体</li>
        <ul>
            <li>font-style</li>
                normal，italic，oblique <br/>
        </ul>
    <li>大小写</li>
        <ul>
            <li>text-transform</li>
                uppercase,lowercase,capitalize <br/>
        </ul>
    <li>下划线、删除线</li>
        <ul>
            <li>text-decoration</li>
                none,underline,overline，line-through，blink <br/>
        </ul>
    <li>行间距</li>
    line-height, 一般设定在1.4em~1.5em
    <li>字母间距和单词间距</li>
    - letter spacing<br/>
    - word spacing, 通常设定为0.25em<br/>
    <li>对齐方式</li>
        <ul>
            <li>text-align</li>
                left, right, center, justify(两端对齐) <br/>
        </ul>
    <li>垂直对其 vertical-align，常应用于<img>元素</li>
    <li>文本缩进 text-indent</li>
        eg：text-indent：20px
    <li>投影 text-shadow</li>
    <li>首字母或首行文本</li>
    eg: p.intro.first-letter {font-size:200%;}<br/>
    eg：p.intro.first-line{font-weight:bold;}
    <li>链接样式 ：link，：visited</li>
    <li>相应用户:hover, :active, :focus </li>
</ul>

## 盒子
<ul>
<li>盒子大小</li>
    <ul>
    <li>盒子大小：width，height</li>
    <li>宽度限制：min-width，max-width</li>
    <li>高度限制：min-height, max-height</li>
    <li>内容溢出：overflow： hidden，scroll</li>
    </ul>
<li>边框</li>
    <ul>
    <li>边框宽度：border-width</li>
        可以用像素值，也可以用：thin，medium，thick<br/>
        也可以通过四个设定，顺序为上，右，下，左<br/>
        eg:border-width:1px 4px 12px 4px;
    <li>边框样式：border-style</li>
        <table>
            <th scope="col">属性</th>
            <th scope="col">说明</th>
            <tr>
                <td>solid</td>
                <td>实线</td>
            </tr>
            <tr>
                <td>dotted</td>
                <td>方形点虚线</td>
            </tr>
                <td>dashed</td>
                <td>虚线</td>
            <tr>
                <td>double</td>
                <td>双实线</td>
            </tr>
                <td>groove</td>
                <td>刻入的凹槽</td>
            <tr>
                <td>ridge</td>
                <td>凸起</td>
            </tr>
                <td>inset</td>
                <td>嵌入屏幕</td>
            <tr>
                <td>outset</td>
                <td>突出屏幕</td>
            </tr>
        </table>
    <li>边框颜色：border-color</li>
    <li>快捷方式：border</li>
        按照宽度、样式、颜色设置；<br/>
        border：3px dotted #0088dd
     <li>内边距：padding</li>
     <li>外边距：margin</li>
     <li>内容居中</li>
        让盒子在页面上居中，left-margin和right-margin设置为auto
     <li>内联元素和块级元素转换：display</li>
        inline，块级变内联<br/>
        block，内联变块级<br/>
        inline-block<br/>
        none，隐藏盒子，区别于visibility的hidden，盒子仍占位置，但是不显示内容<br/>
        以上，不能在内联盒子中创建块级元素<br/>
        eg：导航条<br/>
        li {diplay：inline； margin-right：10px}
     <li>边框图像：border-image</li>
     <li>盒子投影：box-shadow</li>
     <li>圆角：border-radius</li>
        通过1个像素值设计圆角；<br/>
        通过2个像素值设计椭圆角；<br/>
    </ul>
</ul>

## 表格
<ul>
    <li>项目符号样式：list-style-type</li>
        <ul>
            <li>无序列表：属性值设定</li>
                - none <br/>
                - disc 原点<br/>
                - circle 原圈<br/>
                - square 正方形<br/>
            <li>有序列表</li>
                - decimal (1 2 3)<br/>
                - decimal-leading-zero (01 02 03)<br/>
                - lower-alpha (a b c)<br/>
                - upper-alpha (A B C)<BR/>
                - lower-roman<br/>
                - upper-roman<br/>
        </ul>
    <li>项目图像:list-style-image</li>
        eg:list-style-image:url("images/star.png");
    <li>标记的定位：list-style-position</li>
        <ul>
            <Li>outside,标记在文本段落的外面</li>
            <Li>inside，标记在文本段落包围</li>
        </ul>
    <li>列表快捷方式：list-style</li>
        eg：list-style: inside circle width: 300px;
    <li>表格属性</li>
        <ul>
            <Li>width 表格宽度</li>
            <Li>padding 边框和内容的空隙</li>
            <Li>text-transform 转为大写</li>
            <li>letter-spacing,font-size</li>
            <li>border-top，border-bottom上下方边框</li>
            <li>text-align对齐</li>
            <li>background-color 交替改变表格行的背景颜色</li>
            <li>：hover光标悬浮显示</li>
        </ul>
    <li>空单元格的边框:empty-cells</li>
        <ul>
        <li>show，hide</li>
        <li>inhert嵌套的表格的样式，遵循外部表格规则</li>
        </ul>
     <li>单元格之间的空隙:border-spacing,border-collapse</li>
        <ul>
        <li>collapse</li>
        <li>separate</li>
        </ul>
     <li>光标样式:cursor</li>
       
</ul>

## 布局
<ul>
    <li>css定位机制</li>
        <ul>
        <li>普通流：依次换行</li>
        <li>相对定位：相对原来的位置进行移动</li>
        <li>绝对定位：脱离文档流，不占原空间，由祖先元素决定位置</li>
        z-index属性控制盒子图层
        </ul>
    <li>普通流：position：static，默认，可以不必声明</li>
    <li>相对定位：position：relative</li>
        使用top/bottom,left/right属性控制
    <li>绝对定位：position：absolute</li>
        使用top/bottom,left/right属性控制
    <li>固定定位：position：fixed</li>
        在视窗中的位置被固定
    <li>重叠元素：z-index</li>
        数值越大，越在上面
    <li>浮动元素：float</li>
        普通流中的元素在它包含的元素内尽可能向左或向右排列。
    <br/><br/>
    <li>清除浮动：Clear</li>
        left、right、both、none属性值；盒子不允许左或者右接触任何浮动元素；
</ul>