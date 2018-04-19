# font-min-cut
7000常用汉字精简+特殊字符


### 使用`font-spider`提取字符
在index.html中已经包含了7000常用汉字和一些常见字符。
`fonts`目录下已经准备好了`微软雅黑`的几个字体文件。
项目当中我们使用`MicrosoftYaHeiUILight`当常规字体，`MicrosoftYaHei`当粗体。

1. 指定要提取的字体文件，修改`font-face`中的`url`为所需要提取的字体文件路径。
```css
@font-face {
    src: url('./MicrosoftYaHeiUILight.ttf') format('truetype');
}
```
2. `./node_modules/.bin/font-spider index.html`，会得到提取之后的字体ttf。

3. `font-sipder`提取之后缺少空格，可以使用[fontcreator](http://www.high-logic.com/font-editor/fontcreator.html)对字体就行编辑，手动添加空格或者从文字的字体文件中copy空格过来。
