
## 致谢

 **（1）字体**

- 落霞孤鹜（LXGW） - [霞鹜文楷](https://github.com/lxgw/LxgwWenKai) & [霞鹜文楷屏幕阅读版](https://github.com/lxgw/LxgwWenKai-Screen) & [霞鹜文楷 GB](https://github.com/lxgw/LxgwWenkaiGB)

 **（2）工具**

- fontTools - [pyftsubset](https://fonttools.readthedocs.io/en/latest/subset/) & [ttLib.woff2](https://fonttools.readthedocs.io/en/latest/index.html?highlight=woff2#utilities)

- 夜煞之乐2001（NightFurySL2001） - [字体计数软件 CJK-character-count](https://github.com/NightFurySL2001/CJK-character-count)

 **（3）字表**

- 《通用规范汉字表》（8105字）

- 《信息交换用汉字编码字符集 基本集》（GB 2312）（6763字）

  注：额外添加了“〇”。



## 用法

 **（1）字体文件列表**

```
lxgw-wenkai-regular-v1.245.1-full
lxgw-wenkai-regular-v1.245.1-subset-gb2312
lxgw-wenkai-regular-v1.245.1-subset-standard

lxgw-wenkai-gb-regular-v0.965.1-full
lxgw-wenkai-gb-regular-v0.965.1-subset-gb2312
lxgw-wenkai-gb-regular-v0.965.1-subset-standard

lxgw-wenkai-screen-v1.245-full
lxgw-wenkai-screen-v1.245-subset-gb2312
lxgw-wenkai-screen-v1.245-subset-standard

lxgw-wenkai-mono-regular-v1.245.1-full
lxgw-wenkai-mono-regular-v1.245.1-subset-gb2312
lxgw-wenkai-mono-regular-v1.245.1-subset-standard

lxgw-wenkai-mono-gb-regular-v0.965.1-full
lxgw-wenkai-mono-gb-regular-v0.965.1-subset-gb2312
lxgw-wenkai-mono-gb-regular-v0.965.1-subset-standard

lxgw-wenkai-gb-screen-v1.245-full
lxgw-wenkai-gb-screen-v1.245-subset-gb2312
lxgw-wenkai-gb-screen-v1.245-subset-standard
```

 **（2）文件名含义**

- `lxgw-wenkai`：霞鹜文楷

- `regular`：Regular 字重

- `gb`：字形符合国标

- `screen`：更粗的屏幕阅读版

- `mono`：等宽字

- `full`：未子集化的源文件

- `subset`：子集化后的文件

- `v1.245.1 / v1.245 / v0.965.1`：源文件的版本号

- `gb2312`：包含 GB 2312 中的 6763 个字

- `standard`：包含《通用规范汉字表》中的 8105 个字


 **（3）使用**

若要在网页中将该字体用作 WebFont （建议使用 WOFF2 格式），

以 Screen 版为例，可在 CSS 样式表中如此调用：

```css
@font-face {
  font-family: LXGW WenKai Screen;
  font-display: swap;
  src:  local(LXGW WenKai Screen),
        url(/fonts/lxgw-wenkai-screen-v1.245-subset-gb2312.woff2) format(woff2);
}
        /* 浏览器会首先检查本地是否已安装该字体，
           若否，则会从网站根目录的 fonts 文件夹中加载 */

body {
  font-family: LXGW WenKai Screen, system-ui, -apple-system, BlinkMacSystemFont, sans-serif, serif;
}
```


## 其他

~~[前往 npm](https://www.npmjs.com/package/lxgw-wenkai-subset)~~ （已暂停更新）

如有更大的字库需求，可以使用 [霞鹜文楷轻便版](https://github.com/lxgw/LxgwWenKai-Lite/)

只想使用网页字体的话，还可以看看这个 @chawyehsu 制作的 [lxgw-wenkai-webfont](https://github.com/chawyehsu/lxgw-wenkai-webfont)
