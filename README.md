
## 致谢

 **（1）字体**

- 落霞孤鹜(LXGW) - [霞鹜文楷 LXGW WenKai](https://github.com/lxgw/LxgwWenKai) & [霞鹜文楷屏幕阅读版 LXGW WenKai Screen](https://github.com/lxgw/LxgwWenKai-Screen)

 **（2）工具**

- fontTools - [pyftsubset](https://fonttools.readthedocs.io/en/latest/subset/) & [ttLib.woff2](https://fonttools.readthedocs.io/en/latest/index.html?highlight=woff2#utilities)

- 夜煞之乐2001(NightFurySL2001) - [字体计数软件 CJK-character-count](https://github.com/NightFurySL2001/CJK-character-count)

 **（3）字表**

- 《通用规范汉字表》（8105字）

- GB2312 中的汉字（6763字）

  注：额外添加了“〇”。



## 用法

 **（1）文件列表**

```
/* TTF 格式 */
/ttf/lxgwwenkai-regular.original.v1.113.ttf
/ttf/lxgwwenkai-regular.subset.v1.113.gb2312.ttf
/ttf/lxgwwenkai-regular.subset.v1.113.standard.ttf
/ttf/lxgwwenkaiscreen.original.v1.112.ttf （注：Screen 版未发布 v1.113 的小更新）
/ttf/lxgwwenkaiscreen.subset.v1.112.gb2312.ttf
/ttf/lxgwwenkaiscreen.subset.v1.112.standard.ttf

/* WOFF2 格式 */
/woff2/lxgwwenkai-regular.original.v1.113.woff2
/woff2/lxgwwenkai-regular.subset.v1.113.gb2312.woff2
/woff2/lxgwwenkai-regular.subset.v1.113.standard.woff2
/woff2/lxgwwenkaiscreen.original.v1.112.woff2
/woff2/lxgwwenkaiscreen.subset.v1.112.gb2312.woff2
/woff2/lxgwwenkaiscreen.subset.v1.112.standard.woff2

/* 字表 */
/text/gb2312.txt
/text/standard.txt
```

 **（2）文件名**

- 文件名含 `original` 的是 @落霞孤鹜 发布的未子集化的源文件

- 文件名含 `subset` 的是子集化后的文件

- 文件名含 `gb2312` 的字体使用了 GB2312 字库精简

- 文件名含 `standard` 的字体使用了《通用规范汉字表》精简


 **（3）使用**

若要在网页中将该字体用作 WebFont （建议使用 WOFF2 格式），

以 screen 版为例，可在样式表中如此调用：

```css
@font-face {
  font-family: LXGW WenKai Screen;
  font-display: swap;
  src:  local(LXGW WenKai Screen),
        url("/fonts/lxgwwenkaiscreen.subset.v1.112.gb2312.woff2") format("woff2");
}
        /* 浏览器会首先检查本地是否已安装该字体，
           若否，则会从网站根目录的 fonts 文件夹中加载 */

body {
  font-family: LXGW WenKai Screen, system-ui, -apple-system, BlinkMacSystemFont, sans-serif, serif;
}
```

另外也可使用 jsDelivr 的 CDN 服务，

即在上述字体文件列表中需要用到的文件前

添加 `https://cdn.jsdelivr.net/npm/lxgw-wenkai-subset@1.113.0`

然后替换上方示例中的 src 部分，  
即：

```css
  src:  local(LXGW WenKai Screen),
        url(https://cdn.jsdelivr.net/npm/lxgw-wenkai-subset@1.113.0/woff2/lxgwwenkaiscreen.subset.v1.112.gb2312.woff2) format("woff2");
```


## 其他

[前往 npm](https://www.npmjs.com/package/lxgw-wenkai-subset)

如有更大的字库需求，可以使用 [LXGW WenKai Lite / 霞鹜文楷轻便版](https://github.com/lxgw/LxgwWenKai-Lite/)。
