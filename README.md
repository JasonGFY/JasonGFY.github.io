# I want to create my own web page
## Jason Guan
I will use github to manage my web page code and create a public web page for self-presnetation.
right now, my local git files can't synchronize to the remote github.
finally, i find the issue is that the file names were **case-sensitive**

## HTML&CSS Notes
- **结构**<br />
   \<html><br />
        \<body><br />
        \<h1> Main Heading \</h1><br />
        \<p> text paragragh \</p><br />
        \<h2> sub heading \</h2><br />
        \<p>text paragragh\</p><br />
        \</body><br />
    \</html><br />

- ==Notes==<br />
    **标签** \<字符 特性=特性值><br />
            body 所有内容显示在页面中；<br />
            head~title 显示在浏览器顶端；<br />
     - **结构化标记**<br /> 
            h1   一级标题；块级元素另起一行<br />
            h2~6 二至6级标题；块级元素另起一行<br />
            p    段落；块级元素另起一行<br />
            b    粗体<br />
            i    斜体<br />
            sup  上标<br />
            sub  下标<br />
            br / 换行<br />
            hr / 水平线<br />
     - **语义化标记**<br />
            strong  重要，类似于b<br/>
            em      强调，类似于i<br/>
            blockquote cite="" ~ p 较长引用<br/> 
            q 较短引用<br/>
            cite 引用名字<br/>
            dfn 新术语<br/>
            abbr title="" 缩写<br/>
            address 设计者详情<br/>
            del 删除<br/>
            ins 修改时插入的文档<br/>
            s 删除不准确或不想管内容，类似于del<br/>
 - **列表**<br/>
        <ol>
        <li>有序列表:ol li</li>
        <li>无序列表:ul li</li>
        <li>定义列表:dl dt术语 dd定义</li>
         <li>嵌套列表:ul li ul li</li>
        </ol>

<h3>链接</h3>
<hr>

\<a href="http://www.****.com">IMBD\</a><br/>
<ol>
<li>**网页链接**
    <ul>
    <li>a 元素建立链接</li>
    <li>href 特性制定链接的页面</li>
    <li>a尖括号后 是显示的可以指向链接的文字</li>
    </ul>
    <dfn>URL</DFN> uniform resource locator统一资源定位器。<br/>
    *绝对URL* 以网站的域名开头，域名后指定具体页面的路径。没有指定页面会显示主页。<BR/>
    *相对URL*可用于为网站内部的页面之间建立链接。<BR/>
    HTML编写的网站主页通常命名为**index.html**<br>
    <ul>
    <li>相同文件夹：直接使用文件名</li>
    a href="revies.html"
    <li>子文件夹：子文件夹后面夹文件名</li>
    a href="music/lisitings.html
    <li>孙子文件夹</li>
    a href="movies/dvd/reviews.html"
    <li>父文件夹</li>
    a href="../index.html"
    <li>祖父文件夹</li>
    a href="../../index.html"
    </ul>
  </li>
  <li>emial链接 mailto:<br/>
    a href="mailto:someone@example.com"  
  </li>
  <li>新窗口打开链接 target<br/>
    a href="http://www.***.com" target="_blank"
  </li>
  <li>链接到特定位置<br/>
    在链接的目标点设置id，比如： h2 id="introduction"<br/>
    在链接点设置a href #,比如 a href ="#introduction"
  </li>
</ol>      

<h3>图像</h3>
<hr>

\<img src=" " alt=" " title="" height="" width="">
  <ul>
  <li>img元素，向页面中添加图片。</li>
  <li>img必须含有两个特征：src、alt</li>
    <ul>
      <li>src，指向网站中相对UTL的某个图像</li>
      <li>alt,图像的文本描述，可以使用空引号</li>
    </ul>
  <li>title,附件信息，鼠标悬停在图片时会显示</li>
  越来越多的人使用css来指定图片大小
  </ul>

图片在块级元素前，块级元素会另起一行；<br/>
图片在块级元素中，文本会环绕图片；<br/>
  <ul>
  <li>align特性=“left”或者“right”，文字会在图片的左边或有变</li>
  <li>align特性html5之后不再支持</li>
  </ul>

<p>创建图像的三条规则
  <ol>
    <li>正确的格式：jpeg、gif、png</li>
     图片颜色丰富用jpeg；单调用gif或png；
    <li>正确的大小保存</li>
    <li>以像素来衡量图像</li>
  </ol>

<h3>表格</h3>
<hr>

<ul>
<li>基本表格结构 </li>
  <ul>
  <li> table元素创建表格 </li>
  <li> tr 每一行的开始 </li>
  <li> td 每一个单元格的内容 </li>
  <li> th scope ="col" 列标题 </li>
      th scope = "row" 行标题 
  <li> td colspan = "n",单元格横跨n列</li>
      td rowspan = "n",单元格横跨n行
  </ul>
<li>上下长度很长的表格</li>
  <ul>
    <li> thead 放表格标题</li>
    <li> tbody 放表格主体</li>
    <li> tfoot 放表格脚注</li>
  </ul>
</ul>

<h3>表单</h3>
<hr>

<ul>
<li>表单控件 </li>
  <ul>
  <li> 表单控件位于form元素中 </li>
  <li> action特性，服务器上一个一面的URL</li>
  <li> method特性,get 从服务器上检索数据;post 表单中的值在HTTP头信息中进行发送 </li>
  </ul>
<li>单行文本框</li>
  <ul>
    <li> input type="text" name="username" maxlength="10"</li>
      单行文本框，用于数据username的信息，最大程度为10
    </ul>
<li> 密码框</li>
    <ul>
    <li> input type="password" name="password" maxlength=10</li>
    type为password时，文本会被掩盖
  </ul>
  <li> 多行文本框 textarea /</li>
  <li> 单选按钮 input type=“radio”</li>
  <li> 复选框 input=“checkbox”</li>
  <li> 下拉列表框 select option / /</li>
  <li> 多选框 select multiple="multiple"</li>
  <li> 文件上传域 input type=“file”</li>
  <li> 提交按钮 input type="submit" value="subscribe"</li>
  <li> 图像按钮 input type="image" src="相对URL"</li>
  <li> 日期控件 input type= "date"</li>
  <li> 搜索输入控件 input type=“search”</li>
  <li> 组合表单元素 fieldset legend //</li>
</ul>

<h3>其他标记</h3>
<hr>

<ul>
<li>HTML中的注释&lt!-- comments --&gt </li>
<li>每个HTML元素都有的特性 </li>
  <ul>
    <li>id特性</li>
    <li>class特性</li>
  </ul>
<li>块级元素、内联元素<br/>
&ltdiv&gt元素可以将一组元素集中到一个块级元素内<br/>
&ltspan&gt元素可以将若干内联元素内联
</li>
<li>内联框架&ltiframe&gt<br/>网页中分割一个小窗口看到另一个网页<br/>
src="url" scrolling="no"
</li>
<li>页面信息&ltmeta&gt元素位于head元素中，包含所有页面相关信息，通过特性携带信息。name（description、keywords、robots是否加入搜索引擎）、content（robots对应content设定为noindex，不加入搜索结果；设定为nofollow，加入搜索结果，但不要收录页面上其它链接页面）</li>
<li>转意符</li>
  <ul>
    <li> & lt 是小于号</li>
    <li> & gt 是大于号</li>

  </ul>
</ul>