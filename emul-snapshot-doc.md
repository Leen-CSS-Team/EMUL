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

- <font color="red">深色模式目前已停止测试</font>

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

- 小型按钮（small button）

目前为了丰富按钮的多样性与可用性，我们加入了小型按钮来进一步完善按钮

![](https://coding-pages-bucket-126277-7922605-6465-394446-1304367309.cos-website.ap-hongkong.myqcloud.com/EMUL-docs-img/28.png)

```html
<button class="button small blue">测试文字</button>
<button class="button small green">测试文字</button>
<button class="button small yellow">测试文字</button>
<button class="button small red">测试文字</button>
  ```

- pop-ups弹窗

目前全新的pop-ups弹窗的样式只有一个，等到添加进正式版之后会增多。

![](https://coding-pages-bucket-126277-7922605-6465-394446-1304367309.cos-website.ap-hongkong.myqcloud.com/EMUL-docs-img/29.png)

调用方法为：

```html

<div class="container">
  <div class="interior">
    <a class="btn" href="#open-modal">Basic CSS-Only Modal</a>
  </div>
</div>
<div id="open-modal" class="modal-window">
  <div>
    <a href="#" title="Close" class="modal-close">X</a>
    <h1 class="text">成功！</h1>
    <div class="text">我觉得挺好的！哈哈哈哈哈</div>
    <div><small>Check out</small></div>
    </div>
</div>
```

其中，那个“X”实际上是拟UI中的关闭图标。如果你想要改为更加形象的图标，完全可以调用图标库。这里可以推荐<a href="https://icons.bootcss.com/">bootstrap-icons</a>或者<a href="https://www.iconfont.cn/">iconfont</a>

示例：

```html
<div class="container">
  <div class="interior">
    <a class="btn" href="#open-modal">Basic CSS-Only Modal</a>
  </div>
</div>
<div id="open-modal" class="modal-window">
  <div>
    <a href="#" title="Close" class="modal-close">
        <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-x" viewBox="0 0 16 16">
  <path d="M4.646 4.646a.5.5 0 0 1 .708 0L8 7.293l2.646-2.647a.5.5 0 0 1 .708.708L8.707 8l2.647 2.646a.5.5 0 0 1-.708.708L8 8.707l-2.646 2.647a.5.5 0 0 1-.708-.708L7.293 8 4.646 5.354a.5.5 0 0 1 0-.708z"/>
</svg>
<!--这里引用的就是bootstrap的图标库-->
</a>
    <h1 class="text">成功！</h1>
    <div class="text">我觉得挺好的！哈哈哈哈哈</div>
    <div><small>Check out</small></div>
    </div>
</div>
```
![](https://coding-pages-bucket-126277-7922605-6465-394446-1304367309.cos-website.ap-hongkong.myqcloud.com/EMUL-docs-img/30.png)

如果改成文字也是非常行的

```html
<div class="container">
  <div class="interior">
    <a class="btn" href="#open-modal">Basic CSS-Only Modal</a>
  </div>
</div>
<div id="open-modal" class="modal-window">
  <div>
    <a href="#" title="Close" class="modal-close">关闭</a>
    <h1 class="text">成功！</h1>
    <div class="text">我觉得挺好的！哈哈哈哈哈</div>
    <div><small>Check out</small></div>
    </div>
</div>
```

![](https://coding-pages-bucket-126277-7922605-6465-394446-1304367309.cos-website.ap-hongkong.myqcloud.com/EMUL-docs-img/31.png)

这个组件学习了网上的一个版本，并且对其加以改进，比如说颜色、样式、以及对于移动端更加完美的适配。在这里也十分感谢原作者。<a href="https://www.jq22.com/code2521">我最先找到的源地址</a>