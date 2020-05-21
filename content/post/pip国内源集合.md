---
author : "ArnoLiu"
title : "pip国内源集合"
date : "2019-12-27"
description : ""
tags : [
    "pip",
    "linux",
    "环境配制",
]
---

<p>阿里云&nbsp;<a href="http://mirrors.aliyun.com/pypi/simple/" rel="nofollow" target="_blank">http://mirrors.aliyun.com/pypi/simple/</a>&nbsp;<br />&emsp;&emsp;中国科技大学&nbsp;<a href="https://pypi.mirrors.ustc.edu.cn/simple/" rel="nofollow" target="_blank">https://pypi.mirrors.ustc.edu.cn/simple/</a>&nbsp;<br />&emsp;&emsp;豆瓣(douban)&nbsp;<a href="http://pypi.douban.com/simple/" rel="nofollow" target="_blank">http://pypi.douban.com/simple/</a>&nbsp;<br />&emsp;&emsp;清华大学&nbsp;<a href="https://pypi.tuna.tsinghua.edu.cn/simple/" rel="nofollow" target="_blank">https://pypi.tuna.tsinghua.edu.cn/simple/</a>&nbsp;<br />&emsp;&emsp;中国科学技术大学&nbsp;<a href="http://pypi.mirrors.ustc.edu.cn/simple/" rel="nofollow" target="_blank">http://pypi.mirrors.ustc.edu.cn/simple/</a></p>
<hr />
<p>&nbsp;</p>
<p>修改源方法：</p>
<p>临时使用：&nbsp;<br />可以在使用pip的时候在后面加上-i参数，指定pip源&nbsp;<br />例如: pip install scrapy -i&nbsp;<a href="https://pypi.tuna.tsinghua.edu.cn/simple" rel="nofollow" target="_blank">https://pypi.tuna.tsinghua.edu.cn/simple</a></p>
<p>永久修改：&nbsp;<br />linux:&nbsp;<br />修改 ~/.pip/pip.conf (没有就创建一个)， 内容如下：</p>
<div class="cnblogs_code">
<pre>[global]
index-url = https://pypi.tuna.tsinghua.edu.cn/simple</pre>
</div>
<p>windows:&nbsp;<br />直接在user目录中创建一个pip目录，如：C:\Users\xx\pip，新建文件pip.ini，内容如下</p>
<pre>[global]
index-url = https://pypi.tuna.tsinghua.edu.cn/simple</pre>
<p>若要装具体版本，则在包名tensorflow后加上 == 版本号&nbsp; &nbsp;例如：</p>
<div class="cnblogs_Highlighter sh-gutter">
<div>
<div id="highlighter_441466" class="syntaxhighlighter  python">
<table border="0" cellspacing="0" cellpadding="0">
<tbody>
<tr>
<td class="gutter">
<div class="line number1 index0 alt2">1</div>
</td>
<td class="code">
<div class="container">
<div class="line number1 index0 alt2"><code class="python plain">conda install tensorflow</code><code class="python keyword">=</code><code class="python keyword">=</code><code class="python value">1.9</code><code class="python plain">.</code><code class="python value">0</code></div>
</div>
</td>
</tr>
</tbody>
</table>
</div>
</div>
</div>
<p>&nbsp;</p>
<p><em>ps:插一句，当你在找其他的一些conda源、pip源、国内镜像源都没有的包的时候，你可以在<a href="https://pypi.org/" target="_blank">pypi.org</a>上下载到你所需要的包，然后本地安装 :</em></p>
<p><em>pip install 本地路径名.压缩格式</em></p>