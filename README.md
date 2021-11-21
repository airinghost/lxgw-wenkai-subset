
## 致谢

### （1）字体

- 落霞孤鹜(LXGW) - [霞鹜文楷 LXGW WenKai](https://github.com/lxgw/LxgwWenKai)

### （2）工具

- fontTools - [子集化功能 pyftsubset](https://fonttools.readthedocs.io/en/latest/subset/)

- 夜煞之乐2001(NightFurySL2001) - [字体计数软件 CJK-character-count](https://github.com/NightFurySL2001/CJK-character-count)

### （3）字表

- 《通用规范汉字表》一级字、二级字

  注：额外添加了“〇”。



## 用法

### （1）文件列表

```
/* TTF 格式 */
/ttf/lxgw-wenkai.original.v1.110-21.10.14.ttf
/ttf/lxgw-wenkai.subset.6501.char.ttf
/ttf/lxgw-wenkai.subset.6501.char.symbol.ttf
/ttf/lxgw-wenkai-screen.original.v1.110-RC.2.ttf
/ttf/lxgw-wenkai-screen.subset.6501.char.ttf
/ttf/lxgw-wenkai-screen.subset.6501.char.symbol.ttf

/* WOFF2 格式 */
/woff2/lxgw-wenkai.original.v1.110-21.10.14.woff2
/woff2/lxgw-wenkai.subset.6501.char.woff2
/woff2/lxgw-wenkai.subset.6501.char.symbol.woff2
/woff2/lxgw-wenkai-screen.subset.6501.char.woff2
/woff2/lxgw-wenkai-screen.subset.6501.char.symbol.woff2

/* 字表 */
/corpus/general-standard-chinese-characters-table1-table2.txt
/corpus/general-standard-chinese-characters-table1-table2.symbols.txt
```

### （2）文件名

- 文件名含 `original` 的是 @落霞孤鹜 发布的未子集化的源文件，
版本号 v1.110-21.10.14

- 文件名含 `screen` 的是屏幕阅读版，
版本号 v1.110-RC.2

- 文件名含 `subset` 的是子集化后的文件，
汉字数量 6501，
其中：

  `char` 仅包含汉字，

  `char.symbol` 包含汉字与常用符号。

- 本子集化字体目前`不含`拉丁字母与阿拉伯数字。


### （3）使用

《通用规范汉字表》的一、二级字基本可覆盖日常用字，如有更大的字库需求，可以使用 [LXGW WenKai Lite / 霞鹜文楷轻便版](https://github.com/lxgw/LxgwWenKai-Lite/)。

若要在网页中将该字体用作 WebFont （建议使用 WOFF2 格式），

以 screen 版为例，可在样式表中如此调用：

```css
@font-face {
  font-family: LXGW WenKai Screen Subset;
  font-display: swap;
  src:  local(LXGW WenKai Screen),
        local(LXGW WenKai Screen Subset),
        url("/fonts/lxgw-wenkai-screen.subset.6501.char.symbol.woff2") format("woff2");
}
        /* 浏览器会首先检查本地是否已安装该字体，
           若否，则会从网站根目录的 fonts 文件夹中加载 */

body {
  font-family: LXGW WenKai Screen Subset, system-ui, -apple-system, BlinkMacSystemFont, sans-serif, serif;
}
```

另外也可使用 jsDelivr 的 CDN 服务，

即在上述字体文件列表中需要用到的文件前

添加 `https://cdn.jsdelivr.net/npm/lxgw-wenkai-subset@0.5.1`

然后替换上方示例中的 src 部分，
即：

```css
  src:  local(LXGW WenKai Screen),
        local(LXGW WenKai Screen Subset),
        url(https://cdn.jsdelivr.net/npm/lxgw-wenkai-subset@0.5.1/woff2/lxgw-wenkai-screen.subset.6501.char.symbol.woff2) format("woff2");
```



## 其他

版本 `0.5.1`

[前往 npm](https://www.npmjs.com/package/lxgw-wenkai-subset)
