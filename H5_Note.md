##HTML5基础

###样式、链接和表格

####三种样式表插入方式

1，外部样式表
	
	<!-- 写在head中，调用一个外部的css文件，css中设置了style -->
	<link rel="stylesheet" type/css href="mystyle.css"

2，内部样式表
	
	<!-- 写在head中，使用一个css类型，设置了style -->
	<style type="text/css">
	body {
		background-color: red
	}
	p {
		margin-left: 20px
	}
	</style>

3，内联样式表

	<!-- 直接写在标签中，设置了一个style -->
	<a href="newHtml.html" style="color: yellowgreen;">aaa</a>
	
	
####链接

1，文本链接和图片链接

文本

	<!-- 普通的文本链接 -->
	<a href="http://www.baidu.com" style="color: yellowgreen;">
		百度一下
	</a>
	
图片

	<!-- 图片链接 引用了一张图片设置了宽高 设置了当图片无法加载时显示一个自定义的名称 -->
	<a href="http://www.baidu.com">
        <img src="photo.jpg" width="100px" height="100px" alt="html5logo">
    </a>

2，文档内链接
	
	<!-- 通过名称（name）定位到另一个<a> -->
	<a name="tips">This is a Tip</a>
    <a href="#tips">Jump to tip</a>
    

####表格

1，绘制基本的表格

	<!-- 绘制一个基本的表格，一个<tr>标签标示一行，一个<td>标签标示一个单元格 -->
	<table>
        <tr>
            <td>单元格1</td>
            <td>单元格2</td>
        </tr>
    </table>
    
2，多行表格

	<!-- 多个<tr>，绘制多行表格 -->
	<table>
        <tr>
            <td>单元格1</td>
            <td>单元格2</td>
        </tr>
        <tr>
            <td>单元格3</td>
            <td>单元格4</td>
        </tr>
    </table>
    
3，表格的标题

	<!-- 利用<caption>为表格设置标题 -->
	<table>
        <caption>表格标题</caption>
        <tr>
            <td>单元格1</td>
            <td>单元格2</td>
        </tr>
    </table>
    
4，表格的表头

	<!-- 利用<th>为表格设置表头。表头会加自动粗居中显示 -->
	<table>
        <tr>
            <th>第一列</th>
            <th>第二列</th>
        </tr>
        <tr>
            <td>单元格1</td>
            <td>单元格2</td>
        </tr>
    </table>
    
5，边框、表格内容边距、单元格距离和背景颜色

	<!-- 利用border、cellpadding、cellspacing、bgcolor分别设置上述属性 -->
	<table border="1" cellpadding="10" cellspacing="10" bgcolor="#a52a2a">
        <tr>
            <th>第一列</th>
            <th>第二列</th>
        </tr>
        <tr>
            <td>单元格1</td>
            <td>单元格2</td>
        </tr>
    </table>
    
6，表格内标签

	<!-- 在一个单元格（<td>）中，用<ul>表示将要开始绘制表格内标签，用<li>标签表示一条标签 -->
	<table border="1">
        <tr>
            <td>
                <ul>
                    <li>第一项</li>
                    <li>第二项</li>
                </ul>
            </td>
            <td>单元格2</td>
            <td>单元格3</td>
        </tr>
    </table>


###列表、块和布局

####列表

