### 在github上，有些图片可能因为网速原因加载不出来，影响文档体验，你可以选择<a href="https://gitee.com/leen-css-team/EMUL/blob/master/emul-snapshot-doc.md" target="_blank">在gitee查看</a>

# EMUL-snapshot-doc

## EMUL与EMUL-snapshot的区别

- 内容丰富度不同

EMUL的内容相对于EMUL-sna-snapshot更少，EMUL-snapshot的内容更加丰富

- 稳定性不同

EMUL可以看做是一个稳定版本，它的所有内容都是经过测试，十分稳定的；而EMUL-snapshot可看做是一个快照版，他的内容是最新的、最多的，但是他的bug会偏多，且样式也可能相对于EMUL更加粗糙一些

- 更新速度不同

EMUL为了追求稳定性，更新速度将减慢，直至在EMUL-snapshot里的新功能稳定之后才会更新至EMUL。而EMUL-snapshot的更新速度将快一些

## Getting Started

使用EMUL-snapshot同样也可以使用link href引入：

```html
<!--主线-->
<link rel="stylesheet" type="text/css" href="https://leen-css-team.gitee.io/emul/input/emul-snapshot.min.css">

<!--github线路-->
<link rel="stylesheet" type="text/css" href="https://leen-css-team.github.io/EMUL/input/emul-snapshot.min.css">
```

也可以可以git clone本项目，或者通过代码仓库提供的下载按钮下载.zip，然后将<kbd>文件夹css</kbd>中的一些<kbd>.css</kbd>文件引入至你的<kbd>.html</kbd>文件中，即可使用。

## 比普通的EMUL更新了什么

- 增加了dark模式的导航栏

![](https://coding-pages-bucket-126277-7922605-6465-394446-1304367309.cos-website.ap-hongkong.myqcloud.com/EMUL-docs-img/%E6%8D%95%E8%8E%B7.PNG)

全新的dark导航栏

全新的dark导航栏写法如下：

```html
<header class="header-dark">
    测试文字
</header>
```

当然，如果你要使用它，请尽量使用深色背景，EMUL建议使用以下css代码：

```css
 body{
    background-color: #181818;
}
```

- 重点在此，EMUL的dark模式正式测试

目前我们实现夜间模式的办法十分简单粗暴，就是——直接写一个新的css（逃）

目前在css_snapshot里面为夜间模式源码的为：

```
emul_snapshot_background_dark.css

emul_snapshot_button_dark.css

emul_snapshot_miscellaneous_dark.css

emul_snapshot_text_dark.css
```

只要将这四个css文件link引入即可

更加便携的引入方式我们也准备好了，通过以下代码即可引入：

```html
<!--主线-->
<link rel="stylesheet" type="text/css" href="https://leaf2006.gitee.io/emul/input/emul-snapshot-dark.min.css">

<!--github线路-->
<link rel="stylesheet" type="text/css" href="https://leen-css-team.github.io/EMUL/input/emul-snapshot-dark.min.css">
```

为了确保原有功能的完整，全新的夜间模式与原来的夜间模式实现共存

- 全新button（button第一阶段更新）

为了更好的适应移动端，目前EMUL-snapshot测试一种全新的button样式，目前业已完成第一阶段更新，主要更新了小型实心按钮的样式

1.样式改变
全新的样式如下：

<img src="https://coding-pages-bucket-126277-7922605-6465-394446-1304367309.cos-website.ap-hongkong.myqcloud.com/EMUL-docs-img/25.PNG" >

相比原来的样式，现在的小型按钮更"大”了，且更有移动端（安然：越看越像PC）的味道，并且现在新版的小型实心按钮有着更好的文字支持，同时给黄色按钮这种内部文字不容易看清的按钮的内部文字改成了黑色。

2.代码改变

全新的小型实心按钮，去除了后面的"small"字段，所以新版代码如下：

```html
    <button class="solid blue">solid blue</button>
	
    <button class="solid green">solid green</button>
    
    <button class="solid yellow">solid yellow</button>
	
    <button class="solid red">solid red</button>
    
    <button class="solid blue large">solid blue large</button>
	
    <button class="solid green large">solid green large</button>
 
    <button class="solid yellow lage">solid yellow lage</button>
	
    <button class="solid red large">solid red large</button>
```
注：若为中空按钮，请把solid改为hollow
        且顺序可以随意打乱 (添加large则表示字体变大)



- 翻转卡片的更新

在全新版本，我们更新了翻转卡片，效果如下（日常拿安然试验）：

![](https://coding-pages-bucket-126277-7922605-6465-394446-1304367309.cos-website.ap-hongkong.myqcloud.com/EMUL-docs-img/14.gif)

代码实现如下：

```html
<div class="content">
  <div class="card">
    <div class="card-side card-side-front">
      <!-- Front Content -->
      <div class="card-cont">
        <span class="blue">名片封面</span><span>(<span class="green">'写啥都行'</span>)</span>
      </div>
    </div>
    <div class="card-side card-side-back">
      <!-- Back Content -->
      <div class="card-cta">

          <br />
          <span class="space red">名字</span><span class="cyan">:</span> <span class="green">'安然'</span>,
          <br/>
          <span class="space red">邮箱</span><span class="cyan">:</span> <span class="green">不方便透露</span>',
          <br/>
          <span class="space red">工作室</span><span class="cyan">:</span> <span class="green">'**工作室'</span>,
          <br/>
          <span class="space red">网站</span><span class="cyan">:</span> <span class="green">'暂时没有（不存在的）'</span>
         
        </p>
      </div>
    </div>
  </div>
  ```
  
 - 新版本的switch开关（switch第三阶段更新）

新型switch（比leafdeveloper的更为美观“确信”）
- <img src="https://coding-pages-bucket-126277-7922605-6465-394446-1304367309.cos-website.ap-hongkong.myqcloud.com/EMUL-docs-img/26.gif" >
 实现代码：
```html
    <label class="checkbox2switch">
        <input type="checkbox">
        <div class="checkbox2line"><span /></div>
    </label>
```

- Alert Card（第一阶段更新）

目前我们更新了全新的alert card（学习bootcss，哈哈哈）

<img src="https://coding-pages-bucket-126277-7922605-6465-394446-1304367309.cos-website.ap-hongkong.myqcloud.com/EMUL-docs-img/21.gif" >

实现代码：

```html
<div class="alertbox blue">阿巴阿巴</div>
    <div class="alertbox red">阿巴阿巴</div>
```

<img src="https://coding-pages-bucket-126277-7922605-6465-394446-1304367309.cos-website.ap-hongkong.myqcloud.com/EMUL-docs-img/23.gif" >

实现代码：

```html
    <div class="alertbox red">阿巴阿巴</div>
```

感谢Guang_Chen_将调用代码重写一遍，使其更加的简洁！！

- jumbotron

这是全新的“巨幕(Jumbotron)组件。它是一个轻量版的一个巨型卡片。（仿bootcss）

![](https://coding-pages-bucket-126277-7922605-6465-394446-1304367309.cos-website.ap-hongkong.myqcloud.com/EMUL-docs-img/27.png)

```html
<div class="jumbotron">
		<div class="jumbotron-title">Hello World</div>
		<div class="line"></div>
		<div class="jumbotron-text">This is jumbotron from EMUL!</div>
		<button class="solid blue large">Learn more</button>
  </div>
  ```

<b>拆分代码</b>

内部粗体标题文字，请调用：

```html
<div class="jumbotron-title">Add the words do you want</div>
```

内容细体正文文字，请调用：

```html
<div class="jumbotron-text">Add the words do you want
</div>
```

如要分隔标题和正文，可以调用：

```html
<div class="line"></div>
```