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
            h1   一级标题<br />
            h2~6 二至6级标题<br />
            p    段落<br />
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

- **链接**<br/>
\<a href="http://www.****.com">IMBD\</a><br/>
---
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
