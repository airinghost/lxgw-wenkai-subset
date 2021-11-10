
## 1 致谢

### 1.1 字体

- 落霞孤鹜(LXGW) - [霞鹜文楷 LXGW WenKai](https://github.com/lxgw/LxgwWenKai)

### 1.2 工具

- fontTools - [子集化功能 pyftsubset](https://fonttools.readthedocs.io/en/latest/subset/)

- 夜煞之乐2001(NightFurySL2001) - [字体计数软件 CJK-character-count](https://github.com/NightFurySL2001/CJK-character-count)

### 1.3 字表

- 《通用规范汉字表》一级字、二级字

  注：额外添加了“〇”。



## 2 文件

```
### 2.1 文件列表

/* TTF 格式 */
/ttf/lxgw-wenkai.original.v1.110-21.10.14.ttf
/ttf/lxgw-wenkai.subset.6501.char.ttf
/ttf/lxgw-wenkai.subset.6501.char.symbol.ttf

/* WOFF2 格式 */
/woff2/lxgw-wenkai.original.v1.110-21.10.14.woff2
/woff2/lxgw-wenkai.subset.6501.char.woff2
/woff2/lxgw-wenkai.subset.6501.char.symbol.woff2

/* 字表 */
/corpus/general-standard-chinese-characters-table1-table2.txt
/corpus/general-standard-chinese-characters-table1-table2.symbols.txt


### 2.2 说明

文件名含 original 的是 @落霞孤鹜 发布的未子集化的源文件，
版本号 v1.110-21.10.14。

文件名含 subset 的是子集化后的文件，
汉字数量 6501，
其中：
  char 仅包含汉字，
  char.symbol 包含汉字与常用符号。

本子集化字体不含拉丁字母与阿拉伯数字。


### 2.3 使用

若您要使用 WebFont，那么在上述列表中需要用到的文件前
添加 https://cdn.jsdelivr.net/npm/lxgw-wenkai-subset@0.5.0 
即可使用 jsDelivr 的 CDN 全球加速服务，

例如：
https://cdn.jsdelivr.net/npm/lxgw-wenkai-subset@0.5.0/woff2/lxgw-wenkai.subset.6501.char.symbol.woff2

建议使用 WOFF2 格式
```



## 其他

版本 0.5.0

npm 地址 https://www.npmjs.com/package/lxgw-wenkai-subset
