

# EMUL-snapshot-doc

## EMUL与EMUL-snapshot的区别

- 内容丰富度不同

EMUL的内容相对于EMUL-sna-snapshot更少，EMUL-snapshot的内容更加丰富

- 稳定性不同

EMUL可以看做是一个稳定版本，它的所有内容都是经过测试，十分稳定的；而EMUL-snapshot可看做是一个快照版，他的内容是最新的、最多的，但是他的bug会偏多，且样式也可能相对于EMUL更加粗糙一些

- 更新速度不同

EMUL为了追求稳定性，更新速度将减慢，直至在EMUL-snapshot里的新功能稳定之后才会更新至EMUL。而EMUL-snapshot的更新速度将快一些

## Getting Started

使用EMUL-snapshot同样也可以使用link href网页引入：

```html
<!--主线-->
<link rel="stylesheet" type="text/css" href="https://leaf2006.gitee.io/emul/input/emul-snapshot.min.css">

<!--github线路-->
<link rel="stylesheet" type="text/css" href="https://leaf2006.github.io/EMUL/input/emul-snapshot.min.css">
```

也可以可以git clone本项目，或者通过代码仓库提供的下载按钮下载.zip，然后将<kbd>文件夹css</kbd>中的一些<kbd>.css</kbd>文件引入至你的<kbd>.html</kbd>文件中，即可使用。

## 比目前EMUL更新了什么

- 增加了dark模式的导航栏

![](https://ct3fak.coding-pages.com/EMUL-docs-img/%E6%8D%95%E8%8E%B7.PNG)

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
<link rel="stylesheet" type="text/css" href="https://leaf2006.github.io/EMUL/input/emul-snapshot-dark.min.css">
```

为了确保原有功能的完整，全新的夜间模式与原来的夜间模式实现共存