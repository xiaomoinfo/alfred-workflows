# Alfred Workflows

![License MIT](https://img.shields.io/npm/l/express.svg)
![Alfred-Version](https://img.shields.io/badge/Alfred-2.x%7C3.x-lightgrey.svg)

Alfred 是 mac 下最流行的提升效率的工具, 其中 Alfred workflow 又将它自身的强大性能提升了几个数量级. 下面分享几个自主研发的workflow 供大家玩味.

## Finder Path *(v1.0)*

[`[Download Finder Path]`](https://github.com/Louiszhai/alfred-workflows/blob/master/workflows/Finder%20Path.alfredworkflow?raw=true)

通常，获取目录路径可能有以下几个场景：

1. 配置代理，比如说 whistle，配置代理时需要本地文件路径；
2. 需要在终端中打开当前目录，或者操作当前目录；
3. 查看目录路径，用于脚本开发；
4. 其它任何用途；

设置快捷命令后，选中一个目录，按下快捷键，自动获取目录路径并复制到剪切板，然后就可以愉快的使用了（如果目录路径中包含了空格，会自动转义成反斜杆 \ 加空格的形式）。

## Search *(v1.0)*

[`[Download Search]`](https://github.com/Louiszhai/alfred-workflows/blob/master/workflows/Search.alfredworkflow?raw=true)

程序员都离不开搜索, 每天耗费在搜索上的时间更是不计其数. 实际上, 搜索的操作步骤是可以被优化的. `Search` 正是一款这样的workflow. 基于它, 您可以任何区域选中文本, 按下绑定好的快捷键 (最多两次按键, 建议绑定快捷键为Option+W), 便可直接在默认浏览器打开搜索结果页, 省心省力. 目前搜索引擎支持 谷歌, 百度, 雅虎, 维基百科等.

## Shortcuts Query *(v1.0)*

[`[Download Shortcuts Query]`](https://github.com/Louiszhai/alfred-workflows/blob/master/workflows/Shortcuts%20Query.alfredworkflow?raw=true)

`Shortcuts Query` 默认支持 Android Studio 或 WebStorm 快捷键的查询. 除此之外, 该 workflow 还内置了 vim 以及 tmux 共3种快捷键的查询. 

![shortcuts][Shortcuts Query]

同时它还支持其他快捷键的查询, 你唯一需要做的就是参考 `tmux.shortcuts` 文件, 再写一个快捷键对照表, 并将它命名为 "queryName" + ".shortcuts".

![shortcuts][1]    ![shortcuts][2]



## Front End Web Query *(v1.0)*

[`[Download Front End Web Query]`](https://github.com/Louiszhai/alfred-workflows/blob/master/workflows/Front%20End%20Web%20Query.alfredworkflow?raw=true)

前端工程师在开发的过程中经常需要查询一些资料, 几乎每次都要经过 "输入网址—>等待网页打开—>点击输入框—>输入关键字—>按回车查询—>焦急等待查询结果出来" 这样一个漫长的过程, 其中有许多次键盘操作以及鼠标操作, 不但思路容易打断还浪费时间. 我希望的是直接输入关键字, 即刻展示搜索结果, 这便整理了一些常用的网站, 诞生了 `Front End Web Query`, 该 workflow 默认支持4种资源的查询, 包括 mdn, baidu, google, w3c 等, 安装后, 可以自行增加对其他网站的查询. 

- 选中查询结果按shift键可以预览网页
- 按Enter键将在默认浏览器上直接打开网页

mdn search

![shortcuts][Front End Web Query01]

baidu search

![shortcuts][Front End Web Query02]

google search 需要翻墙, 天朝的GFW, 你懂得.

![shortcuts][Front End Web Query03]

w3c search 默认搜索html的便签, 可以自行更改查询的链接实现对其他 w3c 网站的查询, 为加快对搜索结果的展示, w3c search 默认开启了缓存机制, 更新查询链接后, 需要手动运行一次 "w3school().setAlfredCache()" (w3school.py源码中注释的部分).

![shortcuts][Front End Web Query04]

除去上述列出的几项, `Front End Web Query` 还新增了对 [pc6 下载站](http://www.pc6.com/), [Linux命令大全](http://man.linuxde.net/) 等网站的搜索.

## qrcode *(v1.0)*

选中任意文本, 生成相应二维码, 并在默认浏览器中打开二维码.

[`[Download qrcode]`](https://github.com/Louiszhai/alfred-workflows/blob/master/workflows/qrcode.alfredworkflow?raw=true)

如下便是一个使用该workflow生成的二维码图片.

![shortcuts][qrcode]

## License


Released under [MIT](http://rem.mit-license.org/)  LICENSE.



[Shortcuts Query]: images/shortcuts01.png
[Front End Web Query01]: images/shortcuts02.png
[Front End Web Query02]: images/shortcuts03.png
[Front End Web Query03]: images/shortcuts04.png
[Front End Web Query04]: images/shortcuts05.png
[qrcode]: images/qrcode.png
[1]: images/shortcuts-step01.png
[2]: images/shortcuts-step02.png
