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

