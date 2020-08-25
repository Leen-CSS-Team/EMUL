

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
<link rel="stylesheet" type="text/css" href="https://txh0dp.coding-pages.com/input/emul-snapshot.min.css">
```

也可以可以git clone本项目，或者通过代码仓库提供的下载按钮下载.zip，然后将<kbd>文件夹css</kbd>中的一些<kbd>.css</kbd>文件引入至你的<kbd>.html</kbd>文件中，即可使用。

## 比目前EMUL更新了什么

- 更加简单的导航栏写法

原先，我们写导航栏需使用以下代码：（蓝色导航栏）

```html
<header class="header-blue">
    <div class="header-title-
    white">测试文字</div>
</header>
```

而现在EMUL-snapshot的写法可直接如下：

```html
<header class="header-blue">
    测试文字
</header>
```

中间省去了以下代码：
```html
<div class="header-title-white">测试文字</div>
```

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

