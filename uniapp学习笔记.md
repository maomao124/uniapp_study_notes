<h1 style="font-size:3em;color:skyblue;text-align:center">uniapp学习笔记</h1>

[toc]

---











# 概述

uni-app 是一个使用 Vue.js 开发所有前端应用的框架，开发者编写一套代码，可发布到iOS、Android、Web（响应式）、以及各种小程序（微信/支付宝/百度/头条/飞书/QQ/快手/钉钉/淘宝）、快应用等多个平台

即使不跨端，`uni-app`也是更好的小程序开发框架、更好的App跨平台框架、更方便的H5开发框架



## 特点

`uni-app`在开发者数量、案例、跨端抹平度、扩展灵活性、性能体验、周边生态、学习成本、开发成本等8大关键指标上拥有更强的优势



* 开发者/案例数量更多

* 平台能力不受限：在跨端的同时，通过条件编译+平台特有API调用，可以优雅的为某平台写个性化代码，调用专有能力而不影响其他平台

* 性能体验优秀：加载新页面速度更快、自动diff更新数据，App端支持原生渲染，可支撑更流畅的用户体验

* 周边生态丰富

* 学习成本低：基于通用的前端技术栈，采用vue语法+微信小程序api，无额外学习成本

* 开发成本低：不止开发成本，招聘、管理、测试各方面成本都大幅下降





## 功能框架图

![img](img/uniapp学习笔记/uni-function-diagram.png)









# HBuilderX

## 概述

HBuilderX是通用的前端开发工具，但为uni-app做了特别强化

HBuilderX，H是HTML的首字母，Builder是构造者，X是HBuilder的下一代版本。我们也简称HX。 HX是轻如编辑器、强如IDE的合体版本



## 特点

1. 轻巧 仅10余M的绿色发行包(不含插件)
2. 极速 不管是启动速度、大文档打开速度、编码提示，都极速响应 C++的架构性能远超Java或Electron架构
3. vue开发强化 `HX`对vue做了大量优化投入，开发体验远超其他开发工具
4. 小程序支持 国外开发工具没有对中国的小程序开发优化，`HX`可新建`uni-app` `小程序`等项目，为国人提供更高效工具
5. markdown利器 `HX`是唯一一个新建文件默认类型是markdown的编辑器，也是对md支持最强的编辑器 `HX`为md强化了众多功能
6. 清爽护眼 HX的界面比其他工具更清爽简洁，绿柔主题经过科学的脑疲劳测试，是最适合人眼长期观看的主题界面
7. 强大的语法提示 `HX`是中国唯一一家拥有自主IDE语法分析引擎的公司，对前端语言提供准确的代码提示和[转到定义](https://hx.dcloud.net.cn/Tutorial/UserGuide/goto?id=转到定义)(Alt+鼠标左键)
8. 高效极客工具 更强大的多光标、智能双击...让字处理的效率大幅提升
9. 更强的json支持 现代js开发中大量json结构的写法，`HX`提供了比其他工具更高效的操作







## 安装

以Windows为例



**下载**

HBuilderX下载地址: [下载地址](https://www.dcloud.io/hbuilderx.html)

### 

**解压**

HBuilderX，Windows为zip包，解压后才能使用



**创建快捷方式**

![image-20231114163042674](img/uniapp学习笔记/image-20231114163042674.png)







**启动**

HBuilderX，首次启动后，您会看到一个选择窗口，您可以在此选择您喜欢的主题、快捷键







## 入门

### 新建项目

![image-20231114164609791](img/uniapp学习笔记/image-20231114164609791.png)



选择一个模板

![image-20231114164646649](img/uniapp学习笔记/image-20231114164646649.png)



![image-20231114164808585](img/uniapp学习笔记/image-20231114164808585.png)





![image-20231114164900303](img/uniapp学习笔记/image-20231114164900303.png)





### 运行项目

![image-20231114170122045](img/uniapp学习笔记/image-20231114170122045.png)



点击运行到内置浏览器





### 语法提示

框架语法提示库是在页面的右下角选择

![image-20231114170520685](img/uniapp学习笔记/image-20231114170520685.png)



![image-20231114170534734](img/uniapp学习笔记/image-20231114170534734.png)





### 代码助手

可以按`alt+数字`选择直接选择某个项目，类似中文输入法数字选词

![image-20231114170705276](img/uniapp学习笔记/image-20231114170705276.png)







### 语法帮助

光标放到某api处，按下F1，就可跳转到这个api的官方手册。目前支持vue、uni-app、5+等api



![image-20231114172032329](img/uniapp学习笔记/image-20231114172032329.png)







### 多光标

hx支持多光标，按 `ctrl+鼠标左键` 就可增加一个光标，`ctrl+鼠标右键` 可取消一个光标或选区





![image-20231114172204970](img/uniapp学习笔记/image-20231114172204970.png)



还可以选择相同词。`ctrl+e` (mac是`cmd+d`)可选中相同的词做批处理



![image-20231114172239593](img/uniapp学习笔记/image-20231114172239593.png)





### 列选择

hx的列选择，是alt+鼠标拖选。或者用快捷键ctrl+alt+↑或↓



### 选择编码、着色高亮

当你打开一个不认识的文档时，即hx的无法高亮着色，可以在右下角选择使用其他编辑器打开。

当你打开一个文件编码错乱，产生乱码时，也可以在右下角选择编码重新打开。



![image-20231114172427098](img/uniapp学习笔记/image-20231114172427098.png)





### 转到定义

转到定义是非常常用的功能，普通编辑器不长于此，只能猜单词跳转。

HBuilderX有强大的语法分析引擎，可以准确的跳转定义位置。

转到定义的快捷键是`Alt+d`，鼠标操作是alt+左键单击



![image-20231114172638579](img/uniapp学习笔记/image-20231114172638579.png)





而HBuilderX还有一个特色是`转到定义到分栏`，`ctrl+alt+左键`，可以把一个定义处的代码打开在另一侧，方便共同查看



![image-20231114172748620](img/uniapp学习笔记/image-20231114172748620.png)





在HBuilderX中，`Alt+Left`或点击工具栏上的`<`, 即可回到上一个光标位置





### 文件快速打开

在顶部工具栏直接搜索工程下的文件名并打开，或者使用快捷键`ctrl+p`





### 目录内搜索

项目管理器点右键，选：查找字符串(当前目录)，可在该目录下所有文件中搜索字符串



![image-20231114173043223](img/uniapp学习笔记/image-20231114173043223.png)



点击支付搜索

![image-20231114173106196](img/uniapp学习笔记/image-20231114173106196.png)





### 缩进调整

hx默认使用`tab`缩进，`tab`长度为4个空格

如果你需要调整缩进长度，比如`tab`长度为2个空格，在工具设置-编辑器中调整

![image-20231114173233198](img/uniapp学习笔记/image-20231114173233198.png)



![image-20231114173243018](img/uniapp学习笔记/image-20231114173243018.png)





如果不喜欢使用tab而喜欢使用空格，也可以在设置中调。注意这个调节只是编辑器里敲tab按键时转为了空格，格式化时仍是tab。





### 语法校验

hx的语法校验都是插件，在工具插件安装中选择各种校验插件，不同语言的校验插件不一样。安装校验插件后，保存文件时会自动执行语法校验

校验概要结果会显示在状态栏，可以按`F4`切换到不同的错误处





### svn/git项目导入

新建项目时选择左下方

![image-20231114173612962](img/uniapp学习笔记/image-20231114173612962.png)



![image-20231114173642838](img/uniapp学习笔记/image-20231114173642838.png)



![image-20231114173700045](img/uniapp学习笔记/image-20231114173700045.png)



也可以在左边导入

![image-20231114173727923](img/uniapp学习笔记/image-20231114173727923.png)







## 设置

Windows: 顶部菜单【工具】-> 【设置】(快捷键: ctrl + alt + ,)



![image-20231114173949952](img/uniapp学习笔记/image-20231114173949952.png)





设置视图，主要分为5部分：

- 常用配置
- 编辑器配置
- 运行配置：手机/模拟器运行和浏览器运行相关配置
- 插件配置：已安装的插件扩展配置
- 源码视图：json文件，包含以上自定义的配置





### 常用配置项

- 编辑器字体大小
- 项目管理器字体大小
- 编辑字体
- 制表符长度
- 空格代替制表符
- 失去焦点自动保存：默认未开启，如需要，请手动开启
- 语言关联配置
- 项目管理器过滤器配置
- 搜索默认不包含的目录：搜索时默认不包含`.git`、`.cvs`、`.svn`、`node_modules`、`unpackage`
- 打开终端数量：最多允许打开的终端数量，默认8
- 本地历史记录
- 项目管理器单击展开/折叠目录（备注：若关闭此项则是双击展开/折叠目录）
- 项目管理器点击目录时打开内部资源管理器 (即点击时，是否打开内置资源管理器)







### 编辑器配置

- 自动换行: 默认不换行，如需要，请启用。
- 高亮时显示空白字符：默认启用。
- 显示换行符
- 选择默认换行符
- 迷你地图最大像素宽度：默认100
- 鼠标悬停预览
- 关闭时记忆文档折叠状态
- 启动.editorconfig支持：默认启用
- 显示代码缩进对齐线
- 显示长行指示竖线
- 长行指示竖线显示在第几列： 默认值80
- 编辑器行高：文档行间距比例，默认1.2
- 仅在选择一个完整的单词时触发相同词高亮
- 启动代码助手：默认启用，可手动关闭
- Tab键自动插入代码助手选中项
- 代码助手字体大小：默认12
- 代码助手触发字符
- 启用px转rem提示
- 启用px转rpx/upx提示 
- 自动匹配匹配字符
- 中文标点免干扰输入
- 文字分隔符
- 插入多光标使用的修饰键
- 使用Ctrl+鼠标滚轮缩放编辑器
- 智能计算制表符长度
- 编辑器向下滚动一屏







## 主题

### 选择主题

1. 在HBuilderX中，您可以点击顶部菜单【工具】【主题】，选择切换您喜欢的主题颜色。
2. HBuilderX内置了3个主题, 分别为`绿柔` `雅蓝` `酷黑`



![image-20231115115531270](img/uniapp学习笔记/image-20231115115531270.png)







### 自定义窗体主题

在文件setting.json的源码视图中，通过定义"workbench.colorCustomizations"字段来自定义您喜欢的主题颜色



```json
"workbench.colorCustomizations": {
    "[Default]": {//绿柔
        "sideBar.background":"#faf6e6", //加深项目管理器颜色
        "editor.background":"#faf6e6" //加深编辑区域背景颜色
    },
    "[Monokai]": {//酷黑
        "toolBar.background": "#272822", //工具栏背景色设为黑色
        "sideBar.background":"#272822" //项目管理器背景色设为黑色
    },
    "[Atom One Dark]": {//雅蓝
        "sideBar.background": "#282c34", //项目管理器背景色设为与代码区背景色相同
        "editor.background":"#282c3f" //调亮编辑区域背景颜色
    }
}
```







## 快捷键

HBuilderX，预设了5种快捷键方案，分别为: `HBuilderX`、`VS Code`、`Sublime Text`、`IntelliJ Idea / Webstorm`、`Eclipse`

![image-20231115154529431](img/uniapp学习笔记/image-20231115154529431.png)







## 鼠标滚轮

|   向上    |      向下      |                |
| :-------: | :------------: | :------------: |
|   Ctrl    |      放大      |      缩小      |
|    Alt    |  向上滚动一屏  |  向下滚动一屏  |
|   Shift   |  向左滚动3列   |  向右滚动3列   |
| Alt+Shift |  向左滚动一屏  |  向右滚动一屏  |
| Ctrl+Alt  | 向左切换选项卡 | 向右切换选项卡 |









## 项目

### 导入项目/目录

点击顶部菜单【文件】【导入】，或点击菜单【打开目录】，即可导入项目到HBuilderX

![image-20231115154911849](img/uniapp学习笔记/image-20231115154911849.png)







### 关闭项目

当项目管理器，项目数量过多时，您可以`关闭项目`

在项目管理器，选中项目，右键菜单，点击【关闭项目】，即可将目移动到【已关闭项目】列表中。

当然，后期也可以从【已关闭项目】中，将需要的项目打开，移动到项目管理器

![image-20231115155045813](img/uniapp学习笔记/image-20231115155045813.png)



![image-20231115155113530](img/uniapp学习笔记/image-20231115155113530.png)





### 项目别名

HBuilderX，支持对项目创建或修改`别名`

项目管理器，选中项目，右键菜单，点击【修改项目别名】，即创建别名

![image-20231115155211043](img/uniapp学习笔记/image-20231115155211043.png)







## 智能双击

在HBuilderX中，但凡特殊点的字符，都能智能双击。

- 双击引号/括号内侧，是选中引号/括号内的内容
- 双击逗号两侧，是选择逗号前一段或后一段
- 双击行尾，是选中该行(不含回车符)
- 双击连词符（-_）选中整个词
- 双击折叠行首内容开头，选择折叠段落
- 双击行首缩进，选择相同缩进的段落
- 双击列表符号，选择列表段落
- 双击Tag开头或结尾，选择整段Tag
- 双击属性赋值等号=，选择Html属性
- 双击if、function等关键字，选择整段包围区域
- 双击分号，选择js等语言的;分号前段落
- 双击css类名左侧，选择Css类
- 双击注释符选择注释区域
- 双击#选择markdown标题段落
- 双击语法定义符开头选择markdown图片、超链接、加粗、倾斜、代码等语法区







## 同时注释if段首尾

if块的调整很常见，除了包围、反包围外，常用操作还有同时注释掉if段首尾。

1. 双击if选中if代码块
2. 按`Ctrl+\`在选区首尾加光标，变成多光标模式
3. 按`Ctrl+/`注释掉选区首尾行







## 跳转/转到定义

### 上一个光标位置

在HBuilderX中，`Alt+Left` (MacOSX: `ctrl + -`)、点击工具栏上的`<`, 即可回到上一个光标位置



### 转到行

转到行快捷键：`ctrl + G`

![image-20231116171036774](img/uniapp学习笔记/image-20231116171036774.png)



![image-20231116171053566](img/uniapp学习笔记/image-20231116171053566.png)



HBuilderX 3.1.13+版本，支持输入0跳转到首行、输入$跳转到最后一行



### 转到定义

转到定义的快捷键是`Alt+d`，鼠标操作是alt+左键单击



### 转到定义到分栏

`ctrl+alt+左键`，可以把一个定义处的代码打开在另一侧，方便共同查看





## 查找替换

### 快速查找文件

`ctrl+p (MacOSX: ⌘P)`，可以定位到搜索框，输入文件名，快速打开任何文件。

文件名后，敲击空格，输入项目名称，可以只搜索指定项目下文件

按住`Ctrl+Tab`, 可以查看在编辑器中，打开的所有文件的列表



### 查找索引符号

在当前文件，按下`Ctrl + Shift + O`, 可以查找索引符号





### 查找字符串

ctrl +F

- 范围：字符串查找，支持`按当前文件`、`按目录`、`按左侧选中`、`按当前项目`、`按所有项目`进行搜索查找。
- 功能：字符串查找，支持`整词匹配`、`正则匹配`、`大小写匹配`，且支持`排除`特定目录



### 区域内搜索

支持选中一段文字，在顶部搜索栏选中区域搜索【Ctrl+Shift+f】，可以在特殊背景区内`搜索`、`替换`、`全选相同词`





## 折叠

折叠的快捷键是`alt+-`和`=`。

或点击`行号`右边的`-`或`+`，即可完成折叠展开。





## 格式化

格式化快捷键, win：`ctrl + K`； mac: `command + K`



### 格式化插件

| 插件名称         | 对应插件配置中的名称    | 是否内置         | 可格式化的文件                             | 插件市场                                             | 插件教程                                                     |
| ---------------- | ----------------------- | ---------------- | ------------------------------------------ | ---------------------------------------------------- | ------------------------------------------------------------ |
| js-beautify      | format                  | 内置插件         | vue、html、js、css、json                   |                                                      | [文档](https://hx.dcloud.net.cn/Tutorial/extension/js-beautify) |
| prettier         | format-prettier         | 非内置，需要下载 | less、sass、vue、stylus(vue内嵌)、ts、yaml | [下载地址](https://ext.dcloud.net.cn/plugin?id=2025) | [文档](https://hx.dcloud.net.cn/Tutorial/extension/prettier) |
| stylus-supremacy | format-stylus-supremacy | 非内置，需要下载 | 格式化单独stylus文件                       | [下载地址](https://ext.dcloud.net.cn/plugin?id=2039) | [文档](https://ext.dcloud.net.cn/plugin?id=2039)             |





1. 当同时存在`js-beautify`和`format-prettier`插件是，格式化`vue`文件，调用的是`format-prettier`插件
2. `stylus-supremacy`只支持格式化独立的stylus文件，如需格式化vue文件内的stylus代码，需要同时安装prettier插件
3. 本地插件目录：HBuilderX所有的插件，都存放于本地`plugins`目录下





### 格式化插件配置

点击菜单【工具】【设置 -> 插件配置】，选择相应插件, 点击`配置文件`进行配置





## 语法校验

代码语法校验，需要安装相应插件



### 语法校验插件

|        语言        |      插件名称      |                           插件地址                           |                           插件文档                           |
| :----------------: | :----------------: | :----------------------------------------------------------: | :----------------------------------------------------------: |
|        html        |   validate-html    | [下载地址](https://ext.dcloud.net.cn/plugin?name=validate-html) | [文档教程](https://hx.dcloud.net.cn/Tutorial/extension/validate-html) |
| css/less/sass/scss | validate-stylelint | [下载地址](https://ext.dcloud.net.cn/plugin?name=validate-stylelint) | [文档教程](https://hx.dcloud.net.cn/Tutorial/extension/validate-stylelint) |
|         js         |     eslint-js      | [下载地址](https://ext.dcloud.net.cn/plugin?name=eslint-js)  | [文档教程](https://hx.dcloud.net.cn/Tutorial/extension/eslint-js) |
|        vue         |     eslint-vue     | [下载地址](https://ext.dcloud.net.cn/plugin?name=eslint-vue) | [文档教程](https://hx.dcloud.net.cn/Tutorial/extension/eslint-vue) |





### 使用方法

在对应的文件上，右键菜单，点击【验证本文档语法】

校验概要结果会显示在`状态栏`

比如有2个错误（如下图），可以按`F4`切换到不同的错误处



![image-20231116172739241](img/uniapp学习笔记/image-20231116172739241.png)







## 文件对比

项目管理器，选中两个要对比的文件，右键菜单，点击【对比选中文件】



![image-20231116173304097](img/uniapp学习笔记/image-20231116173304097.png)







## 本地历史记录

HBuilderX，文件修改、保存时在本地进行备份，防止意外丢失，可通过 “本地历史记录”查看备份文件

在编辑器打开的文件上，点击右键菜单，点击【本地历史记录】



![image-20231116173424251](img/uniapp学习笔记/image-20231116173424251.png)



![image-20231116173451112](img/uniapp学习笔记/image-20231116173451112.png)





菜单【设置】【常用设置】，可以配置`本地历史记录`

- 单个文件最大备份数量
- 单个文件大小限制
- 最长保存时间



![image-20231116173623448](img/uniapp学习笔记/image-20231116173623448.png)









## editorconfig

### 概述

很多公司都要求各开发成员使用相同的编码风格，比如缩进是空格还是tab。

`editorconfig`是一套解决这个问题的业内通用规范，通过在项目下存放配置文件`.editorconfig`，并在这个配置文件中描述规则，然后把这个配置文件和其他代码一起提交git/svn，所有项目成员，都会遵循相同的编码规范。

`editorconfig`可以帮助开发者在不同的编辑器和IDE之间定义和维护一致的代码风格。 `editorconfig`包含一个用于定义代码格式的文件和一批编辑器插件，这些插件可以让编辑器读取配置文件并依此格式化代码。 `editorconfig`的配置文件十分易读，并且可以在各个操作系统、编辑器下工作





### 示例

`jQuery`在`Github`上的`.editorconfig`配置文件如下：



```sh
root = true

[*]
indent_style = tab
end_of_line = lf
charset = utf-8
trim_trailing_whitespace = true
insert_final_newline = true

[package.json]
indent_style = space
indent_size = 2
```





用于设置Python和JavaScript行尾和缩进风格的配置文件：

```sh
# EditorConfig is awesome: http://EditorConfig.org

# top-most EditorConfig file
root = true

# Unix-style newlines with a newline ending every file
[*]
end_of_line = lf
insert_final_newline = true

# 4 space indentation
[*.py]
indent_style = space
indent_size = 4

# Tab indentation (no size specified)
[*.js]
indent_style = tab

# Indentation override for all JS under lib directory
[lib/**.js]
indent_style = space
indent_size = 2

# Matches the exact files either package.json or .travis.yml
[{package.json,.travis.yml}]
indent_style = space
indent_size = 2
```





### 在哪里存放配置文件

当打开一个文件时，`editorconfig`插件会在打开文件的目录和其每一级父目录查找.`editorconfig`文件，直到有一个配置文件`root=true`

如果一个工程中出现多个配置文件，EditorConfig配置文件的读取层级是自上而下的，最深层的配置文件，最后读取。配置规则也是 按照读取的顺序来生效，所以路径上离代码最近的配置规则，优先级最高。





### 文件格式详情

`editorconfig`文件使用INI格式（译注：请参考维基百科），目的是可以与Python ConfigParser Library兼容，但是允许在分段名（译注：原文是section names）中使用“and”。 分段名是全局的文件路径，格式类似于`gitignore`。斜杠`/`作为路径分隔符，`#`或者`;`作为注释。注释应该单独占一行。`editorconfig`文件使用`UTF-8`格式、`CRLF`或`LF`作为换行符。



|   通配符   |                 说明                 |
| :--------: | :----------------------------------: |
|     *      |       匹配除/之外的任意字符串        |
|     **     |            匹配任意字符串            |
|     ？     |           匹配任意单个字符           |
|   [name]   |             匹配name字符             |
|  [!name]   |            匹配非name字符            |
| {s1,s3,s3} | 匹配任意给定的字符串（0.11.0起支持） |



特殊字符可以用`\`转义，以使其不被认为是通配符



|         属性说明         |                             说明                             |
| :----------------------: | :----------------------------------------------------------: |
|       indent_style       |               tab为hard-tabs，space为soft-tabs               |
|       indent_size        | 设置整数表示规定每级缩进的列数和soft-tabs的宽度（译注：空格数）。如果设定为tab，则会使用tab_width的值（如果已指定） |
|        tab_width         | 设置整数用于指定替代tab的列数。默认值就是indent_size的值，一般无需指定。 |
|       end_of_line        |                定义换行符，支持lf、cr和crlf。                |
| trim_trailing_whitespace |     设为true表示会除去换行行首的任意空白字符，false反之      |
|   insert_final_newline   |        设为true表明使文件以一个空白行结尾，false反之         |
|           root           | 表明是最顶层的配置文件，发现设为true时，才会停止查找.`editorconfig`文件。 |



1. 所有的属性名和属性值对`大小写不敏感`。通常，如果没有明确指定某个属性，则会使用编辑器的配置，而`editorconfig`不会处理。
2. 推荐不要指定某些`editorconfig`属性。比如，tab_width不需要特别指定，除非它与`indent_size`不同。同样的，当`indent_style`设为`tab`时，不需要配置`indent_size`，这样才方便阅读者使用他们习惯的缩进格式。另外，如果某些属性并没有规范化（比如`end_of_line`），就最好不要设置它。





### 启用或关闭

在【设置】中，有个editorconfig开关



![image-20231117160912369](img/uniapp学习笔记/image-20231117160912369.png)









## 外部命令

### 使用场景

- 压缩文件与解压
- 压缩图片
- 文档转换（比如markdown转pdf）
- 调用python、shell脚本
- 打开本地的某个程序
- 传输文件到服务器
- 操作服务器的某些服务（如启动、停止、重启nginx)
- 下载文件
- 安装apk到手机
- 上传应用到应用分发网站（比如蒲公英）
- 批量压缩
- 其它的自动化操作
- 上传文件到七牛云、阿里云等





### 外部命令在哪里？

菜单【工具】-->【外部命令】

点击菜单【工具】-->【外部命令】-->【自定义外部命令】，就可以自定义外部命令，格式为json



![image-20231117161151753](img/uniapp学习笔记/image-20231117161151753.png)







### 示例

模板如下：

```sh
//配置外层为数组结构，数组内可添加多个外部命令设置

//外部命令可以让您在HBuilderX中通过菜单、快捷键等方式调用外部程序或命令行

//注意: 左侧为教程，不是配置，需在右侧用户设置中添加外部命令才生效

[
    //------------外部命令 配置属性说明------------//
    {
        //名称，用于在“工具-运行外部命令”菜单中显示
        "name":"Echo",

        //需要执行的外部命令及参数：
        // - 值支持string 和 array 两种形式 
        // - 填写path环境中包含的命令或具体的程序路径及参数
        // - 支持使用变量

        // - command值为string: 命令与参数连写，命令或参数包含空格时需要使用\"\"包围
        "command":"echo ${file}",

        // - command值为array: 命令与参数分开写，命令或参数包含空格时不需要额外处理
        "command": ["C:/Program Files (x86)/Google/Chrome/Application/chrome.exe", "${file}"],

        //运行的环境 [可选项]：
        // - process(默认值): 后台运行，运行时不显示输入输出
        // - shell: 在cmd这样的独立shell环境下运行，运行时会打开shell窗口
        // - terminal: 在HBuilderX自带的内置终端插件中运行
        "type" : "shell",

        //工作目录 [可选项]：命令运行时的工作目录，默认是文件所在目录
        // - 支持使用变量
        "workingDir" : "",

        //快捷键 [可选项] : 可通过此快捷键直接运行此外部命令
        "key": "ctrl+r"
    },

    //------------外部命令 变量说明------------//
    //'command'、'workingDir'中可使用预定义的变量来获取当前文件的路径信息
    // - ${file}             当前文件的完整路径,            比如 D:\\files\\test.txt
    // - ${fileName}         当前文件的文件名,              比如 test.txt
    // - ${fileExtension}    当前文件的扩展名,              比如 txt
    // - ${fileBasename}     当前文件仅包含文件名的部分,     比如 test
    // - ${fileDir}          当前文件所在目录的完整路径,     比如 D:\\files
    // - ${projectDir}       当前文件所在项目的完整路径,     只有当前文件是项目管理器中某个项目下的文件时才起作用

    //------------外部命令 示例------------//
    //1. 在独立shell窗体下使用dir命令打印当前文件所在目录下文件列表
    {
        "name":"Dir",
        "command":"dir ${fileDir}",
        "type": "shell"
    },
    //2. 如安装了Android Studio，可以在avd中新建一个模拟器，然后在HBuilderX中使用快捷键将模拟器直接启动而不必启动AS。注意该终端关闭会导致模拟器关闭，所以更适合在HBuilderX的内置终端中打开
    {
        "name":"Android模拟器",
        "command":"C:\\Users\\username\\AppData\\Local\\Android\\sdk\\emulator\\emulator.exe -netdelay none -netspeed full -avd Nexus_5X_API_27_x86",
        "type" : "terminal",
        "key":"alt+shift+e"
    }

]

```







压缩、解压：

```sh
[{
    "name": "文件: 压缩7z格式",
    "command": "\"C:/Program\ Files/7-Zip/7z.exe\" a ${file}.7z ${file}",
    "type": "process",
    "key": ""
  },
  {
    "name": "文件: 压缩zip格式",
    "command": [
      "C:/Program Files/7-Zip/7z.exe",
      "a",
      "${file}.zip",
      "${file}"
    ],
    "type": "process",
    "key": ""
  },
  {
    "name": "文件: 解压",
    "command": "\"C:/Program Files/7-Zip/7z.exe\" x ${file}",
    "type": "shell",
    "key": ""
  }
]
```





![image-20231117161907654](img/uniapp学习笔记/image-20231117161907654.png)







调用外部python、shell等脚本

```sh
[{
  "name":"调用python脚本",
  "command":"python script.py",
  "type" : "terminal",
  "key":"alt+shift+p"
  }]
```







## 终端

### 安装内置终端

点击顶部菜单【工具 - 插件安装】，打开插件安装窗口，选择`内置终端`，点击安装



![image-20231117162505913](img/uniapp学习笔记/image-20231117162505913.png)







### 启动终端

HBuilderX支持通过多种方式打开终端：

- 左侧视图（项目管理器），选中项目，右键菜单【使用命令行窗口打开所在目录】
- 顶部菜单【视图 - 显示终端】
- 底部状态栏，点击终端图标
- 快捷键方式：Windows (Alt+C); MacOSX (Ctrl+Shift+C)





## 代码块

### 概述

代码块是快速开发的利器。简单的敲几个字母，回车，就能生成大段代码。

比如我们经常会敲if...else结构，在HBuilderX中，只需敲`ife`回车，就能直接生成相应的代码结构。

![image-20231117163340535](img/uniapp学习笔记/image-20231117163340535.png)



回车后生成if结构体



### 常用代码块列表

- iff ：简单if
- forr ：for循环结构体
- fori ：for循环结构体并包含i
- funn：函数
- funa：匿名函数
- clog：打印日志
- clogvar：打印变量命名和值



- dg ：document.getElementById
- dl ：$("")



敲v，即可拉出各种vue代码块





### 代码块设置

查看内建的代码块，点击菜单-工具-代码块设置，选择你要查看的语言的代码块



![image-20231117163853804](img/uniapp学习笔记/image-20231117163853804.png)







### 自定义代码块

自定义代码块都是配置json文件中的

ife的示例如下：

```json
{
"if ... else": {
    "body": [
        "if ($1) {",
        "\t$0",
        "} else{",
        "\t",
        "}"
    ],
    "prefix": "ife",
    "scope": "source.js"
}
}
```





|    配置项     |                             说明                             |
| :-----------: | :----------------------------------------------------------: |
|      key      | 代码块显示名称，显示在代码助手列表中的名字。key是不能重复的。上面例子中`"if ... else"`就是一个`key`。 |
|    prefix     |     代码块的触发字符，就是敲什么字母可以激活这个代码块。     |
|     body      |                         代码块的内容                         |
| triggerAssist | 为`true`表示该代码块输入到文档后立即在第一个`tabstop`上触发代码提示，拉出代码助手，默认为`false`。 |
|    project    | 将代码块控制在指定项目类型下生效。可取值有：`uni-app`、`Web`、`App`、`Wap2App`。 `Web`指普通项目，`App`指5+App项目。如果不设置，则该代码块在所有项目类型下均生效。 比如：`"project": "uni-app"`，代表这个代码块仅在uni-app项目下生效。 如需设置多种项目类型，用逗号分隔。比如：`"project": "uni-app,App"` |



**配置项body详细说明:**

- `$1` 表示代码块输入后光标的所在位置。如需要多光标，就在多个地方配置`$1`；如该位置有预置数据且需要选中，则写法是`${1:selectedtext}`；这里还支持下拉候选菜单，多选项即下拉候选列表使用`${1:foo1/foo2/foo3}`
- `$2` 表示代码块输入后再次按tab后光标的切换位置`tabstops`（代码块展开后按tab可以跳到下一个`tabstop`，在HBuilderX中看到类似绿色光标的不闪的竖线，就可以按tab或回车跳转光标过去）
- `$0`代表代码块输入后最终光标的所在位置（也可以按回车直接跳过去）。









## vue doc

### 概述

可以理解为，vue`组件`使用说明。

在其它文件，使用`组件`的时候，弹出代码提示。





### 支持的标签

**主要用在`script`部分，需要写在`export default`上面**



|    标签     |                             用法                             |                             说明                             |
| :---------: | :----------------------------------------------------------: | :----------------------------------------------------------: |
| description |                @description 这是一个描述信息                 |                        一个组件描述。                        |
|  tutorial   |  @tutorial [https://www.dcloud.io](https://www.dcloud.io/)   |                   用于引用其他文档或教程。                   |
|  property   |                    @property {type} name                     |                     用于描述组件的属性。                     |
|    value    |                 @value 描述属性能够使用的值                  |  值域，用于限定属性能够使用的值。它紧跟在property后面使用。  |
|    event    | @event {(e:MouseEvent)=>void} 事件名称 @event {Function} 事件名称 | 用于提示事件说明。 有两种使用方式, 可写死Function, 也可以写箭头函数。 |
|   example   |  @example `<Pagination @total="50" @close=""></Pagination>`  | 用于提供示例代码。它可以包含一段代码片段，用于演示如何使用注释的代码。可以多行，支持 markdown 语法。 |
| uniPlatform | @uniPlatform {"web": {"uniVer": "3.6.2+", "unixVer": "x" }}  | 仅用于提供uniapp兼容性信息。 `uniPlatform`需要参考详细规范。**`3.9.0+版本后支持`** |





### 示例

```vue
/**
 * 翻页组件
 * @description 翻页组件
 * @tutorial http://www.baidu.com
 * @property {Number} total 翻页数据总数
 * @property {String} size  组件大小
 * @value big 大
 * @value small 小
 * @event {(e:MouseEvent)=>void} open 事件名称
 * @event {Function} close 关闭事件
 * @example <Pagination @total="50" @close=""></Pagination>
 * @uniPlatform {
 *   "app": {
 *     "android": {
 *       "osVer": "8.0",
 *       "uniVer": "3.7.0",
 *       "unixVer": "3.9.0"
 *     },
 *     "ios": {
 *       "osVer": "8.0",
 *       "uniVer": "3.7.0",
 *       "unixVer": "3.9.0"
 *     }
 *   },
 *   "mp": {
 *     "weixin": {
 *       "hostVer": "8.0",
 *       "uniVer": "3.7.0",
 *       "unixVer": "x"
 *     },
 *     "kuaishou": {
 *       "hostVer": "8.0",
 *       "uniVer": "3.7.0",
 *       "unixVer": "x"
 *     }
 *   },
 *   "web": {
 *     "uniVer": "3.6.2+",
 *     "unixVer": "x"
 *   }
 * }
 */
export default {
    props: {
        total: Number,
        size: String,
    },
    data() {
        return {
            pageSize: 10,
            pageNumber: 0,
        };
    },
    methods: {
        handleChange(data, event) {
            this.$emit('PsPn', this.pageSize, this.pageNumber);
        },
    },
};
```









## JSDoc

### 概述

**JSDoc有2个作用，导出API文档和明确代码类型，辅助代码提示。**

JSDoc描述了函数或变量的功能、值域、示例等很多代码提示时需要的数据，还可以通过类型定义，给动态的JS变量或函数赋予明确的类型。

- 对于普通开发者，书写JSDoc有助于代码可读性的提升，在很多要求严格的大公司，JSDoc是强制要求编写的。 完善的JSDoc也能让开发者自定义的函数在引用时得到更方便的代码提示。
- 对于框架开发者，书写好的JSDoc是必须的，除了生成API手册，良好的JSDoc可以让框架在IDE里得到更好的提示。



敲`/**`回车即可生成JSDoc注释模板





### 支持的标签

|                             标签                             |                          用法                          |                       说明                        |
| :----------------------------------------------------------: | :----------------------------------------------------: | :-----------------------------------------------: |
| [description](https://hx.dcloud.net.cn/Tutorial/Language/jsdoc?id=description) |                   @description 内容                    |              描述。支持markdown语法               |
| [example](https://hx.dcloud.net.cn/Tutorial/Language/jsdoc?id=example) |                        @example                        |      示例代码，可以多行，支持 markdown 语法       |
| [param](https://hx.dcloud.net.cn/Tutorial/Language/jsdoc?id=param) |              @param {Type} paramName 描述              |              可以指定参数类型及描述               |
| [property](https://hx.dcloud.net.cn/Tutorial/Language/jsdoc?id=property) |             @property {Type} propName 描述             |            可以指定对象属性类型及描述             |
| [value](https://hx.dcloud.net.cn/Tutorial/Language/jsdoc?id=value) |                    @value value描述                    | 变量支持的值域，需要紧跟在@property或者@param后面 |
| [defaultValue](https://hx.dcloud.net.cn/Tutorial/Language/jsdoc?id=defaultvalue) |                  @defaultValue value                   |                      默认值                       |
| [remark](https://hx.dcloud.net.cn/Tutorial/Language/jsdoc?id=remark) |                      @remark 内容                      |  提供注意事项说明，可以多行，支持 markdown 语法   |
| [return](https://hx.dcloud.net.cn/Tutorial/Language/jsdoc?id=return) |                       {属性类型}                       |                 描述函数的返回值                  |
| [since](https://hx.dcloud.net.cn/Tutorial/Language/jsdoc?id=since) |                           无                           |  版本号 从哪个 HBuilderX 或者编译器版本开始支持   |
| [tutorial](https://hx.dcloud.net.cn/Tutorial/Language/jsdoc?id=tutorial) |                     @tutorial url                      |                   引用教程文档                    |
| [type](https://hx.dcloud.net.cn/Tutorial/Language/jsdoc?id=type) |                      @type {Type}                      |                  描述变量的类型                   |
| [uniPlatform](https://hx.dcloud.net.cn/Tutorial/Language/jsdoc?id=uniplatform) | `@uniPlatform { "app":{...},"mp":{...},"web":{...}} }` |      用于提供兼容性信息。仅用于`uni-app`项目      |







### 示例



```js
/**
 * @description 这是一个动物的构建函数
 */
function Animal(name, weight) {
    this.name = name;
    this.weight = weight;
}
```



```js
/**
 * @description 这是一个构造函数
 * @example
 * 函数使用示例：
 * var animal = new Animal('cat', 10);
 */
function Animal(name,weight){
    this.name = name;
    this.weight = weight;
}
```











## 常用插件

### validate-html

html语法校验插件，需要到[插件市场](https://ext.dcloud.net.cn/plugin?name=validate-html)安装



安装完成后，进入【设置】【插件配置】【htmlhintrc】，点击htmlhintrc, 即可配置相关规则

|           选项           |                           说明                           |
| :----------------------: | :------------------------------------------------------: |
|    tagname-lowercase     |        标签名是否开启小写; true:启用, false:禁用         |
|      attr-lowercase      |        属性名是否开启小写，true:启用, false:禁用         |
| attr-value-double-quotes |    属性值是否必须放在双引号中，true:启用, false:禁用     |
|      doctype-first       | Doctype是否必须是HTML文档的第一行，true:启用, false:禁用 |
|         tag-pair         |         标签是否必须成对，true:启用, false:禁用          |
|     spec-char-escape     |       特殊字符是否必须转义，true:启用, false:禁用        |
|        id-unique         |        ID属性是否必须唯一，true:启用, false:禁用         |
|      src-not-empty       |          src属性是否为空，true:启用, false:禁用          |
|   attr-no-duplication:   |  同一标签中，属性值是否不可重复, true:启用, false:禁用   |





### validate-stylelint

validate-stylelint, 用于校验css、less、scss语法

此插件，需要到[插件市场](https://ext.dcloud.net.cn/plugin?name=validate-stylelint)安装







### eslint-js

eslint-js, 用于校验js和html中的js代码

[eslint-js插件安装地址](https://ext.dcloud.net.cn/plugin?id=2037)





### eslint-vue

此插件用于vue语法校验。[eslint-vue插件安装地址](https://ext.dcloud.net.cn/plugin?id=2005)





### js-beautify

HBuilderX 3.7.6+, 内置format插件(即js-beautify)，支持项目下格式化配置.jsbeautifyrc文件

只有项目下存在`.jsbeautifyrc`文件时才会生效。否则则采用HBuilderX内置的jsbeautifyrc格式化规则





### Formator-Prettier

此插件用于格式化less、sass、vue、stylus、ts、yaml代码

此插件需要到[插件市场](https://ext.dcloud.net.cn/plugin?id=2025)下载。







### compile-node-sass

Scss/Sass 是一款强化 CSS 的辅助工具，它在 CSS 语法的基础上增加了变量 (variables)、嵌套 (nested rules)、混合 (mixins)、导入 (inline imports) 等高级功能，这些拓展令 CSS 更加强大与优雅。

使用 Scss/Sass 以及 Scss/Sass 的样式库（如 Compass）有助于更好地组织管理样式文件，以及更高效地开发项目。

compile-node-sass插件，编译sass/scss为css。

在HBuilderX中，使用`scss/sass`是需要安装`compile-node-sass编译插件`的

安装sass插件，需要到[插件市场](https://ext.dcloud.net.cn/plugin?id=2046)安装



- uni-app项目，会自动编译使用sass的文件。
- 单独编译sass文件。选中sass文件，点击右键菜单 -> 外部命令 -> sass -> 编译scss/sass



点击菜单【工具 -> 插件配置 -> compile-node-sass -> package.json】，即可打开配置文件文件。

打开package.json, 修改key值，即可配置快捷键；可通过此快捷键直接运行此外部命令



点击菜单【工具 -> 插件配置 -> compile-node-sass -> package.json】，即可打开配置文件文件。

配置文件中`onDidSaveExecution`，表示保存的时候是否触发编译，默认为false







### sftp/ftp插件

此插件是vscode中流行的ftp插件，因HBuilderX兼容vscode的部分插件生态，也可以在HBuilderX中使用。

- 使用此插件，可将本地工作区文件，与FTP服务器或linux服务器文件同步。
- 支持`ftp/sftp`协议
- 支持远程文件目录`浏览`、`上传`、`下载`、`删除`
- 支持`自动保存上传`



[SFTP/FTP插件市场插件地址](https://ext.dcloud.net.cn/plugin?id=2038)



1. 在项目管理器，新建一个空目录或空项目，然后选中
2. 右键菜单，点击【Ftp: 创建连接配置】
3. 系统自动创建`.ftp/ftp-sync.json`配置文件
4. 编辑`ftp-sync.json`, 填写`host（ip）`、`username（用户名）`、`password（密码）`、`port（端口）`、`protocol（协议）`
5. 填写完配置文件，右键菜单，点击【Ftp: 浏览远程文件】
6. 选择文件目录，进行`上传`、`下载`、`删除`操作













# uni-app组成和跨端原理

## 基本语言和开发规范

uni-app代码编写，基本语言包括js、vue、css。以及ts、scss等css预编译器。

在app端，还支持原生渲染的nvue，以及可以编译为kotlin和swift的uts。



为了实现多端兼容，综合考虑编译速度、运行性能等因素，`uni-app` 约定了如下开发规范：

- 页面文件遵循 [Vue 单文件组件 (SFC) 规范](https://vue-loader.vuejs.org/zh/spec.html)，即每个页面是一个.vue文件
- 组件标签靠近小程序规范，详见[uni-app 组件规范](https://uniapp.dcloud.net.cn/component/)
- 接口能力（JS API）靠近小程序规范，但需将前缀 `wx`、`my` 等替换为 `uni`，详见[uni-app接口规范](https://uniapp.dcloud.net.cn/api/)
- 数据绑定及事件处理同 `Vue.js` 规范，同时补充了[应用生命周期](https://uniapp.dcloud.net.cn/collocation/App.html#applifecycle)及[页面的生命周期](https://uniapp.dcloud.net.cn/tutorial/page.html#lifecycle)
- 如需兼容app-nvue平台，建议使用flex布局进行开发



uni-app分`编译器`和`运行时（runtime）`。uni-app能实现一套代码、多端运行，是通过这2部分配合完成的



编译器将开发者的代码进行编译，编译的输出物由各个终端的runtime进行解析，每个平台（Web、Android App、iOS App、各家小程序）都有各自的runtime





## 编译器

- 编译器运行在电脑开发环境。一般是内置在HBuilderX工具中，也可以使用独立的cli版。
- 开发者按uni-app规范编写代码，由编译器将开发者的代码编译生成每个平台支持的特有代码
  - 在web平台，将.vue文件编译为js代码。与普通的vue cli项目类似
  - 在微信小程序平台，编译器将.vue文件拆分生成wxml、wxss、js等代码
  - 在app平台，将.vue文件编译为js代码。进一步，如果涉及uts代码：
    - 在Android平台，将.uts文件编译为kotlin代码
    - 在iOS平台，将.uts文件编译为swift代码
- 编译器分vue2版和vue3版
  - vue2版：基于`webpack`实现
  - vue3版：基于`Vite`实现，性能更快
- 编译器支持条件编译，即可以指定某部分代码只编译到特定的终端平台。从而将公用和个性化融合在一个工程中。







## 运行时

runtime不是运行在电脑开发环境，而是运行在真正的终端上。

uni-app在每个平台（Web、Android App、iOS App、各家小程序）都有各自的runtime。这是一个比较庞大的工程。

- 在小程序端，uni-app的runtime，主要是一个小程序版的vue runtime，页面路由、组件、api等方面基本都是转义。
- 在web端，uni-app的runtime相比普通的vue项目，多了一套ui库、页面路由框架、和uni对象（即常见API封装）
- 在App端，uni-app的runtime更复杂，可以先简单理解为DCloud也有一套小程序引擎，打包app时将开发者的代码和DCloud的小程序打包成了apk或ipa



uni-app runtime包括3部分：基础框架、组件、API。



1. 基础框架：
   - 包括语法、数据驱动、全局文件、应用管理、页面管理、js引擎、渲染和排版引擎等
   - 在web和小程序上，不需要uni-app提供js引擎和排版引擎，直接使用浏览器和小程序的即可。但app上需要uni-app提供
   - App的js引擎：App-Android上，uni-app的js引擎是v8，App-iOS是jscore
   - App的渲染引擎：同时提供了2套渲染引擎，`.vue`页面文件由webview渲染，原理与小程序相同；`.nvue`页面文件由原生渲染，原理与react native相同。开发者可以根据需要自主选择渲染引擎。
2. 组件：
   - runtime中包括的组件只有基础组件，如`<view>`、`<button>`等。扩展组件不包含在uni-app的runtime中，而是下载到用户的项目代码中。（这些组件都是vue组件）
   - 为了降低开发者的学习成本，uni-app的内置基础组件命名规范与小程序基本相同。
   - 这几十个组件不管在哪个平台，已被处理为均有一致表现。
   - 在小程序端，uni-app基础组件会直接转义为小程序自己的内置组件。在小程序的runtime中不占体积。
   - 在web和android、iOS端，这几十个组件都在uni-app的runtime中，会占用一定体积，相当于内置了一套ui库。
   - 组件的扩展：
     - 有了几十个基础组件，大多数扩展组件也都是基于这些基础组件封装的。比如官方提供的扩展ui库`uni ui`。
     - 在web平台，for web的各种ui库（如elementUI）也可以使用，但这些库由于操作了dom，无法跨端在app和小程序中使用。
     - 在App平台，uni-app也支持使用原生编程语言来自行扩展原生组件，比如原生的地图、ar等。
     - uni-app同时支持将[微信自定义组件](https://uniapp.dcloud.net.cn/tutorial/miniprogram-subject)运行到微信小程序、web、app这3个平台。注意微信自定义组件不是vue组件。
3. API：
   - uni-app runtime内置了大量常见的、跨端的 [API](https://uniapp.dcloud.net.cn/api/)，比如联网(uni.request)、读取存储(uni.getStorage)
   - 同时uni-app不限制各端原生平台的API调用。开发者可以在uni-app框架中无限制的调用该平台所有能使用的API。即，在小程序平台，小程序的所有API都可以使用；在web平台，浏览器的所有API都可使用；在iOS和Android平台，os的所有API都可以使用。
   - 也就是说，使用uni-app的标准API，可以跨端使用。但对于不跨端的部分，仍可以调用该端的专有API。由于常见的API都已经被封装内置，所以日常开发时，开发者只需关注uni标准API，当需要调用特色端能力时在条件编译里编写特色API调用代码。
   - [ext API](https://uniapp.dcloud.net.cn/api/extapi)：web和app的runtime体积不小，如果把小程序的所有API等内置进去会让开发者的最终应用体积变大。所以有部分不常用的API被剥离为ext API。虽然仍然是uni.开头，但需要单独下载插件到项目下
   - 小程序平台：uni对象会转为小程序的自有对象，比如在微信小程序平台，编写uni.request等同于wx.request。那么所有wx.的API都可以这样使用。
   - web平台：window、dom等浏览器专用API仍可以使用
   - app平台：除了uni.的API，还可以使用[plus.的API](https://www.html5plus.org/doc/h5p.html)、[Native.js](https://uniapp.dcloud.net.cn/tutorial/native-js)，以及通过uts编写原生插件，或者使用java和objectC编写原生插件。这些原生插件调用os的API并封装给js使用。





## 逻辑层和渲染层分离

在web平台，逻辑层（js）和渲染层（html、css），都运行在统一的webview里。

但在小程序和app端，逻辑层和渲染层被分离了。

分离的核心原因是性能。过去很多开发者吐槽基于webview的app性能不佳，很大原因是js运算和界面渲染抢资源导致的卡顿。

不管小程序还是app，逻辑层都独立为了单独的js引擎，渲染层仍然是webview

**所以注意小程序和app的逻辑层都不支持浏览器专用的window、dom等API。app只能在渲染层操作window、dom**，即[renderjs](https://uniapp.dcloud.net.cn/tutorial/renderjs)









# 工程

## 概述

一个 uni-app 工程，就是一个 Vue 项目



## 目录结构

一个uni-app工程，默认包含如下目录及文件：

```sh
┌─uniCloud              云空间目录，阿里云为uniCloud-aliyun,腾讯云为uniCloud-tcb
│─components            符合vue组件规范的uni-app组件目录
│  └─comp-a.vue         可复用的a组件
├─utssdk                存放uts文件
├─pages                 业务页面文件存放的目录
│  ├─index
│  │  └─index.vue       index页面
│  └─list
│     └─list.vue        list页面
├─static                存放应用引用的本地静态资源（如图片、视频等）的目录，注意：静态资源都应存放于此目录
├─uni_modules           存放[uni_module](/uni_modules)。
├─platforms             存放各平台专用页面的目录
├─nativeplugins         App原生语言插件 
├─nativeResources       App端原生资源目录
│  ├─android            Android原生资源目录
|  └─ios                iOS原生资源目录
├─hybrid                App端存放本地html文件的目录
├─wxcomponents          存放小程序组件的目录
├─unpackage             非工程代码，一般存放运行或发行的编译结果
├─AndroidManifest.xml   Android原生应用清单文件
├─Info.plist            iOS原生应用配置文件
├─main.js               Vue初始化入口文件
├─App.vue               应用配置，用来配置App全局样式以及监听 应用生命周期
├─manifest.json         配置应用名称、appid、logo、版本等打包信息
├─pages.json            配置页面路由、导航条、选项卡等页面类信息
└─uni.scss              这里是uni-app内置的常用样式变量
```





## static目录

uni-app编译器根据pages.json扫描需要编译的页面，并根据页面引入的js、css合并打包文件。
对于本地的图片、字体、视频、文件等资源，如果可以直接识别，那么也会把这些资源文件打包进去，但如果这些资源以变量的方式引用， 比如：`<image :src="url"></image>`，甚至可能有更复杂的函数计算，此时编译器无法分析

那么有了static目录，编译器就会把这个目录整体复制到最终编译包内。这样只要运行时确实能获取到这个图片，就可以显示。

当然这也带来一个注意事项，如果static里有一些没有使用的废文件，也会被打包到编译包里，造成体积变大

另外注意，static目录支持特殊的平台子目录，比如web、app、mp-weixin等，这些目录存放专有平台的文件，这些平台的文件在打包其他平台时不会被包含

非 `static` 目录下的文件（vue组件、js、css 等）只有被引用时，才会被打包编译













# 页面

## 概述

uni-app项目中，一个页面就是一个符合`Vue SFC规范`的 vue 文件

在 uni-app js 引擎版中，后缀名是`.vue`文件或`.nvue`文件。 这些页面均全平台支持，差异在于当 uni-app 发行到App平台时，`.vue`文件会使用webview进行渲染，`.nvue`会使用原生进行渲染

一个页面可以同时存在vue和nvue，在[pages.json](https://uniapp.dcloud.net.cn/collocation/pages)的路由注册中不包含页面文件名后缀，同一个页面可以对应2个文件名。重名时优先级如下：

- 在非app平台，先使用vue，忽略nvue
- 在app平台，使用nvue，忽略vue





在 uni-app x 中，后缀名是`.uvue`文件

uni-app x 中没有js引擎和webview，不支持和vue页面并存。

uni-app x 在app-android上，每个页面都是一个全屏activity，不支持透明。





## 新建页面

`uni-app`中的页面，默认保存在工程根目录下的`pages`目录下

每次新建页面，均需在`pages.json`中配置`pages`列表；未在`pages.json -> pages` 中注册的页面，`uni-app`会在编译阶段进行忽略

通过HBuilderX开发 `uni-app` 项目时，在 `uni-app` 项目上右键“新建页面”，HBuilderX会自动在`pages.json`中完成页面注册，开发更方便



![image-20231120101642753](img/uniapp学习笔记/image-20231120101642753.png)





新建页面时，可以选择`是否创建同名目录`。创建目录的意义在于：

* 如果你的页面较复杂，需要拆分多个附属的js、css、组件等文件，则使用目录归纳比较合适
* 如果只有一个页面文件，大可不必多放一层目录





## 删除页面

删除页面时，需做两件工作：

- 删除`.vue`文件、`.nvue`、`.uvue`文件
- 删除`pages.json -> pages`列表项中的配置





## pages.json

pages.json是工程的页面管理配置文件，包括：页面路由注册、页面参数配置（原生标题栏、下拉刷新...）、首页tabbar等众多功能





## 页面生命周期

`uni-app` 页面除支持 Vue 组件生命周期外还支持下方页面生命周期函数，当以组合式 API 使用时，在 Vue2 和 Vue3 中存在一定区别



|               函数名                |                             说明                             |                         平台差异说明                         | 最低版本 |
| :---------------------------------: | :----------------------------------------------------------: | :----------------------------------------------------------: | :------: |
|               onInit                | 监听页面初始化，其参数同 onLoad 参数，为上个页面传递的数据，参数类型为 Object（用于页面传参），触发时机早于 onLoad |                          百度小程序                          |  3.1.0+  |
|               onLoad                | 监听页面加载，该钩子被调用时，响应式数据、计算属性、方法、侦听器、props、slots 已设置完成，其参数为上个页面传递的数据，参数类型为 Object（用于页面传参），参考[示例](https://uniapp.dcloud.net.cn/api/router#navigateto)。 |                                                              |          |
|               onShow                | 监听页面显示，页面每次出现在屏幕上都触发，包括从下级页面点返回露出当前页面 |                                                              |          |
|               onReady               | 监听页面初次渲染完成，此时组件已挂载完成，DOM 树($el)已可用，注意如果渲染速度快，会在页面进入动画完成前触发 |                                                              |          |
|               onHide                |                         监听页面隐藏                         |                                                              |          |
|              onUnload               |                         监听页面卸载                         |                                                              |          |
|              onResize               |                       监听窗口尺寸变化                       |                 App、微信小程序、快手小程序                  |          |
|          onPullDownRefresh          | 监听用户下拉动作，一般用于下拉刷新，参考[示例](https://uniapp.dcloud.net.cn/api/ui/pulldown) |                                                              |          |
|            onReachBottom            | 页面滚动到底部的事件（不是scroll-view滚到底），常用于下拉下一页数据。具体见下方注意事项 |                                                              |          |
|            onTabItemTap             |      点击 tab 时触发，参数为Object，具体见下方注意事项       | 微信小程序、QQ小程序、支付宝小程序、百度小程序、H5、App、快手小程序、京东小程序 |          |
|          onShareAppMessage          |                      用户点击右上角分享                      | 微信小程序、QQ小程序、支付宝小程序、抖音小程序、飞书小程序、快手小程序、京东小程序 |          |
|            onPageScroll             |                  监听页面滚动，参数为Object                  |                          nvue不支持                          |          |
|      onNavigationBarButtonTap       |           监听原生标题栏按钮点击事件，参数为Object           |                           App、H5                            |          |
|             onBackPress             | 监听页面返回，返回 event = {from:backbutton、 navigateBack} ，backbutton 表示来源是左上角返回按钮或 android 返回键；navigateBack表示来源是 uni.navigateBack；[详见](https://uniapp.dcloud.net.cn/tutorial/page.html#onbackpress) |                    app、H5、支付宝小程序                     |          |
|  onNavigationBarSearchInputChanged  |           监听原生标题栏搜索输入框输入内容变化事件           |                           App、H5                            |  1.6.0   |
| onNavigationBarSearchInputConfirmed | 监听原生标题栏搜索输入框搜索事件，用户点击软键盘上的“搜索”按钮时触发。 |                           App、H5                            |  1.6.0   |
|  onNavigationBarSearchInputClicked  | 监听原生标题栏搜索输入框点击事件（pages.json 中的 searchInput 配置 disabled 为 true 时才会触发） |                           App、H5                            |  1.6.0   |
|           onShareTimeline           |                监听用户点击右上角转发到朋友圈                |                          微信小程序                          |  2.8.1+  |
|          onAddToFavorites           |                    监听用户点击右上角收藏                    |                     微信小程序、QQ小程序                     |  2.8.1+  |







## onShow和onHide

页面显示，是一个会重复触发的事件

a页面刚进入时，会触发a页面的onShow

当a跳转到b页面时，a会触发onHide，而b会触发onShow

但当b被关闭时，b会触发onUnload，此时a再次显示出现，会再次触发onShow

在tabbar页面（指pages.json里配置的tabbar），不同tab页面互相切换时，会触发各自的onShow和onHide。





## onInit

- 仅百度小程序基础库 3.260 以上支持 onInit 生命周期
- 其他版本或平台可以同时使用 onLoad 生命周期进行兼容，注意避免重复执行相同逻辑
- 不依赖页面传参的逻辑可以直接使用 created 生命周期替代





## onReachBottom

可在pages.json里定义具体页面底部的触发距离onReachBottomDistance

比如设为50，那么滚动页面到距离底部50px时，就会触发onReachBottom事件。

如使用scroll-view导致页面没有滚动，则触底事件不会被触发





## onPageScroll

|   属性    |  类型  |                 说明                 |
| :-------: | :----: | :----------------------------------: |
| scrollTop | Number | 页面在垂直方向已滚动的距离（单位px） |



```js
onPageScroll : function(e) { //nvue暂不支持滚动监听，可用bindingx代替
	console.log("滚动距离为：" + e.scrollTop);
}
```







## onBackPress

| 属性 |  类型  |                             说明                             |
| ---- | :----: | :----------------------------------------------------------: |
| from | String | 触发返回行为的来源：'backbutton'——左上角导航栏按钮及安卓返回键；'navigateBack'——uni.navigateBack() 方法。**支付宝小程序端不支持返回此字段** |



```js
export default {
	onBackPress(options) {
		console.log('from:' + options.from)
	}
}
```



- `onBackPress`上不可使用`async`，会导致无法阻止默认返回
- 支付宝小程序只有真机可以监听到非`navigateBack`引发的返回事件（使用小程序开发工具时不会触发`onBackPress`），不可以阻止默认返回行为





## onTabItemTap

|   属性   |  类型  |             说明             |
| :------: | :----: | :--------------------------: |
|  index   | Number | 被点击tabItem的序号，从0开始 |
| pagePath | String |   被点击tabItem的页面路径    |
|   text   | String |   被点击tabItem的按钮文字    |



```js
onTabItemTap : function(e) {
	console.log(e);
	// e的返回格式为json对象： {"index":0,"text":"首页","pagePath":"pages/index/index"}
},
```



* onTabItemTap常用于点击当前tabitem，滚动或刷新当前页面。如果是点击不同的tabitem，一定会触发页面切换。
* 如果想在App端实现点击某个tabitem不跳转页面，不能使用onTabItemTap，可以使用plus.nativeObj.view放一个区块盖住原先的tabitem，并拦截点击事件。
* 支付宝小程序平台onTabItemTap表现为点击非当前tabitem后触发，因此不能用于实现点击返回顶部这种操作





## 组件生命周期

`uni-app` 组件支持的生命周期，与vue标准组件的生命周期相同



|    函数名     |                             说明                             | 平台差异说明 | 最低版本 |
| :-----------: | :----------------------------------------------------------: | :----------: | :------: |
| beforeCreate  |                    在实例初始化之前被调用                    |              |          |
|    created    |                  在实例创建完成后被立即调用                  |              |          |
|  beforeMount  |                    在挂载开始之前被调用。                    |              |          |
|    mounted    | 挂载到实例上去之后调用。注意：此处并不能确定子组件被全部挂载，如果需要子组件完全挂载之后在执行操作可以使用`$nextTick` |              |          |
| beforeUpdate  |          数据更新时调用，发生在虚拟 DOM 打补丁之前           | 仅H5平台支持 |          |
|    updated    | 由于数据更改导致的虚拟 DOM 重新渲染和打补丁，在这之后会调用该钩子 | 仅H5平台支持 |          |
| beforeDestroy |         实例销毁之前调用。在这一步，实例仍然完全可用         |              |          |
|   destroyed   | Vue 实例销毁后调用。调用后，Vue 实例指示的所有东西都会解绑定，所有的事件监听器会被移除，所有的子实例也会被销毁 |              |          |







## 页面调用接口

### getApp()

`getApp()` 函数用于获取当前应用实例，一般用于获取globalData。也可通过应用实例调用 `App.vue methods` 中定义的方法

```js
const app = getApp()
console.log(app.globalData)
```



- 不要在定义于 `App()` 内的函数中，或调用 `App` 前调用 `getApp()` ，可以通过 `this.$scope` 获取对应的app实例
- 通过 `getApp()` 获取实例之后，不要私自调用生命周期函数。
- 当在首页`nvue`中使用`getApp()`不一定可以获取真正的`App`对象。对此提供了`const app = getApp({allowDefault: true})`用来获取原始的`App`对象，可以用来在首页对`globalData`等初始化





### getCurrentPages()

`getCurrentPages()` 函数用于获取当前[页面栈](https://uniapp.dcloud.net.cn/tutorial/page.html#页面栈)的实例，以数组形式按栈的顺序给出，数组中的元素为页面实例，第一个元素为首页，最后一个元素为当前页面



每个页面实例的方法属性列表：



| 方法                  | 描述                          | 平台说明 |
| --------------------- | ----------------------------- | -------- |
| page.$getAppWebview() | 获取当前页面的webview对象实例 | App      |
| page.route            | 获取当前页面的路由            |          |



`getCurrentPages()`仅用于展示页面栈的情况，请勿修改页面栈，以免造成页面状态错误。
页面关闭时，对应页面实例会在页面栈中删除



- `navigateTo`, `redirectTo` 只能打开非 tabBar 页面。
- `switchTab` 只能打开 `tabBar` 页面。
- `reLaunch` 可以打开任意页面。
- 页面底部的 `tabBar` 由页面决定，即只要是定义为 `tabBar` 的页面，底部都有 `tabBar`。
- 不能在首页 `onReady` 之前进行页面跳转





### $getAppWebview()

`uni-app` 在 `getCurrentPages()`获得的页面里内置了一个方法 `$getAppWebview()` 可以得到当前webview的对象实例，从而实现对 webview 更强大的控制。在 html5Plus 中，plus.webview具有强大的控制能力

但`uni-app`框架有自己的窗口管理机制，请不要自己创建和销毁webview，如有需求覆盖子窗体上去

**此方法仅 App 支持**







## 页面通讯

### uni.$emit(eventName,OBJECT)

触发全局的自定义事件。附加参数都会传给监听器回调。



|   属性    |  类型  |          描述          |
| :-------: | :----: | :--------------------: |
| eventName | String |         事件名         |
|  OBJECT   | Object | 触发事件携带的附加参数 |





```js
uni.$emit('update',{msg:'页面更新'})
```







### uni.$on(eventName,callback)

监听全局的自定义事件。事件可以由 uni.$emit 触发，回调函数会接收所有传入事件触发函数的额外参数



|   属性    |   类型   |      描述      |
| :-------: | :------: | :------------: |
| eventName |  String  |     事件名     |
| callback  | Function | 事件的回调函数 |





```js
uni.$on('update',function(data){
		console.log('监听到事件来自 update ，携带参数 msg 为：' + data.msg);
	})
```





### uni.$once(eventName,callback)

监听全局的自定义事件。事件可以由 uni.$emit 触发，但是只触发一次，在第一次触发之后移除监听器



|   属性    |   类型   |      描述      |
| :-------: | :------: | :------------: |
| eventName |  String  |     事件名     |
| callback  | Function | 事件的回调函数 |



```js
uni.$once('update',function(data){
		console.log('监听到事件来自 update ，携带参数 msg 为：' + data.msg);
	})
```





### uni.$off([eventName, callback])

移除全局自定义事件监听器



|   属性    |      类型       |      描述      |
| :-------: | :-------------: | :------------: |
| eventName | Array＜String＞ |     事件名     |
| callback  |    Function     | 事件的回调函数 |





- 如果没有提供参数，则移除所有的事件监听器；
- 如果只提供了事件，则移除该事件所有的监听器；
- 如果同时提供了事件与回调，则只移除这个回调的监听器；
- 提供的回调必须跟$on的回调为同一个才能移除这个回调的监听器；







### 示例

`$emit`、`$on`、`$off`常用于跨页面、跨组件通讯



```vue
<template>
	<view class="content">
		<view class="data">
			<text>{{val}}</text>
		</view>
		<button type="primary" @click="comunicationOff">结束监听</button>
		<button type="primary" @click="start()">开始监听</button>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				val: 0
			}
		},
		onLoad() {
			setInterval(() => {
				uni.$emit('add', {
					data: 2
				})
			}, 1000)
			uni.$on('add', this.add)
		},
		methods: {
			comunicationOff() {
				uni.$off('add', this.add)
			},
			add(e) {
			
				this.val += e.data
			},
			start() {
				uni.$on('add', this.add)
			}
		}
	}
</script>

<style>
	.content {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
	}

	.data {
		text-align: center;
		line-height: 40px;
		margin-top: 40px;
	}

	button {
		width: 200px;
		margin: 20px 0;
	}
</style>
```









## 路由

`uni-app`页面路由为框架统一管理，开发者需要在[pages.json](https://uniapp.dcloud.net.cn/collocation/pages#pages)里配置每个路由页面的路径及页面样式。类似小程序在 app.json 中配置页面路由一样。所以 `uni-app` 的路由用法与 `Vue Router` 不同



`uni-app` 有两种页面路由跳转方式：使用[navigator](https://uniapp.dcloud.net.cn/component/navigator)组件跳转、调用[API](https://uniapp.dcloud.net.cn/api/router)跳转。



页面返回时会自动关闭 loading 及 toast, modal 及 actionSheet 不会自动关闭。

页面关闭时，只是销毁了页面实例







## 页面栈

框架以栈的形式管理当前所有页面， 当发生路由切换的时候，页面栈的表现如下：

|  路由方式  |            页面栈表现             |                           触发时机                           |
| :--------: | :-------------------------------: | :----------------------------------------------------------: |
|   初始化   |            新页面入栈             |                   uni-app 打开的第一个页面                   |
| 打开新页面 |            新页面入栈             | 调用 API  [uni.navigateTo](https://uniapp.dcloud.net.cn/api/router#navigateto) 、使用组件  \<navigator open-type="navigate"/> |
| 页面重定向 |     当前页面出栈，新页面入栈      | 调用 API  [uni.redirectTo](https://uniapp.dcloud.net.cn/api/router#redirectto) 、使用组件 \<navigator open-type="redirectTo"/> |
|  页面返回  |   页面不断出栈，直到目标返回页    | 调用 API  [uni.navigateBack](https://uniapp.dcloud.net.cn/api/router#navigateback)  、使用组件 \<navigator open-type="navigateBack"/> 、用户按左上角返回按钮、安卓用户点击物理back按键 |
|  Tab 切换  | 页面全部出栈，只留下新的 Tab 页面 | 调用 API  [uni.switchTab](https://uniapp.dcloud.net.cn/api/router#switchtab) 、使用组件 \<navigator open-type="switchTab"/> 、用户切换 Tab |
|   重加载   |   页面全部出栈，只留下新的页面    | 调用 API  [uni.reLaunch](https://uniapp.dcloud.net.cn/api/router#relaunch) 、使用组件  \<navigator open-type="reLaunch"/> |













# 互相引用

## 引用组件

传统vue项目开发，引用组件需要`导入 - 注册 - 使用`三个步骤

```vue
<template>
	<view>
		<!-- 3.使用组件 -->
		<uni-rate text="1"></uni-rate>
	</view>
</template>
<script>
	// 1. 导入组件
	import uniRate from '@/components/uni-rate/uni-rate.vue';
	export default {
		components: { uniRate } // 2. 注册组件
	}
</script>
```



`uni-app`的`easycom`机制，将组件引用进一步优化，开发者只管使用，无需考虑导入和注册

```vue
<template>
	<view>
		<!-- 1.使用组件 -->
		<uni-rate text="1"></uni-rate>
	</view>
</template>
<script>
</script>
```



在 uni-app 项目中，页面引用组件和组件引用组件的方式都是一样的（可以理解为：页面是一种特殊的组件），均支持通过 `easycom` 方式直接引用





## 引用js

### 引入

`js`文件或`script`标签内（包括 renderjs 等）引入`js`文件时，可以使用相对路径和绝对路径

```js
// 绝对路径，@指向项目根目录，在cli项目中@指向src目录
import add from '@/common/add.js';
// 相对路径
import add from '../../common/add.js';
```



- js 文件不支持使用`/`开头的方式引入





### NPM支持

uni-app支持使用**npm**安装第三方包。



若项目之前未使用npm管理依赖（项目根目录下无package.json文件），先在项目根目录执行命令初始化npm工程：

```sh
npm init -y
```



cli项目默认已经有package.json了。HBuilderX创建的项目默认没有，需要通过初始化命令来创建



在项目根目录执行命令安装npm包：

```sh
npm install xxx --save
```



安装完即可使用npm包，js中引入npm包：

```js
import package from 'xxx'
const package = require('xxx')
```



node_modules 目录必须在项目根目录下。不管是cli项目还是HBuilderX创建的项目







## 引用css

使用`@import`语句可以导入外联样式表，`@import`后跟需要导入的外联样式表的相对路径，用`;`表示语句结束

```vue
<style>
    @import "../../common/uni.css";

    .uni-card {
        box-shadow: none;
    }
</style>
```







## 静态资源

`template`内引入静态资源，如`image`、`video`等标签的`src`属性时，可以使用相对路径或者绝对路径

```html
<!-- 绝对路径，/static指根目录下的static目录，在cli项目中/static指src目录下的static目录 -->
<image class="logo" src="/static/logo.png"></image>
<image class="logo" src="@/static/logo.png"></image>
<!-- 相对路径 -->
<image class="logo" src="../../static/logo.png"></image>
```





`css`文件或`style标签`内引入`css`文件时（scss、less 文件同理），可以使用相对路径或绝对路径

```js
/* 绝对路径 */
@import url('/common/uni.css');
@import url('@/common/uni.css');
/* 相对路径 */
@import url('../../common/uni.css');
```











# js语法

## 标准js和浏览器js的区别

`uni-app`的js代码，h5端运行于浏览器中。非h5端（包含小程序和App），Android平台运行在v8引擎中，iOS平台运行在iOS自带的jscore引擎中，都没有运行在浏览器或webview里

非H5端，虽然不支持window、document、navigator等浏览器的js API，但也支持标准ECMAScript

所以uni-app的非H5端，一样支持标准js，支持if、for等语法，支持字符串、数字、时间、布尔值、数组、自定义对象等变量类型及各种处理方法。仅仅是不支持window、document、navigator等浏览器专用对象



## ES6支持

uni-app 在支持绝大部分 ES6 API 的同时，也支持了 ES7 的 await/async





## Android平台

JS脚本运行在独立Google V8引擎中，版本与Chrome83一致，因此支持的语法与Android系统版本无关

vue页面渲染在系统Webview中，受Android系统版本影响，在Android低端机上存在css浏览器兼容性问题，太新的css语法在低版本不支持

nvue页面使用系统原生View渲染





## iOS平台

JS脚本运行在iOS操作系统提供的JavaScriptCore 引擎，因此支持的语法与iOS系统有关，跟iOS系统的Safari浏览器一致

vue页面渲染在系统WKWebview中，受iOS系统版本影响，兼容性与iOS系统的Safari浏览器一致

nvue页面使用系统原生View渲染









# TypeScript支持

uni-app 支持使用 ts 开发

类型定义文件由 @dcloudio/types 模块提供，安装后请注意配置 tsconfig.json 文件中的 compilerOptions > types 部分



在 vue 或 nvue 页面的 script 节点，添加属性 `lang="ts"`

```vue
<script lang="ts">
    
</script>
```



在根目录创建 `tsconfig.json` 文件，并进行个性化配置

```json
{
  "compilerOptions": {
    "target": "esnext",
    "module": "esnext",
    "strict": true,
    "jsx": "preserve",
    "moduleResolution": "node",
    "esModuleInterop": true,
    "sourceMap": true,
    "skipLibCheck": true,
    "importHelpers": true,
    "allowSyntheticDefaultImports": true,
    "useDefineForClassFields": true,
    "resolveJsonModule": true,
    "lib": [
      "esnext",
      "dom"
    ],
    "types": [
      "@dcloudio/types"
    ]
  },
  "exclude": [
    "node_modules",
    "unpackage",
    "src/**/*.nvue"
  ]
}
```





uni-app 的 vue2 模式：nvue 文件中不支持编写 ts。vue 文件中可以使用 ts，但 ts 版本根据项目类型有区别。HBuilderX 创建的项目使用 ts 3.7.5，cli 创建的项目使用 ts 4.x

uni-app 的 vue3 模式：vue 文件及 nvue 文件均支持最新版 ts













# 条件编译

