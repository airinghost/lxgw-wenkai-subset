
## 1 致谢

### 1.1 字体文件

- 落霞孤鹜(LXGW) - [霞鹜文楷 LXGW WenKai](https://github.com/lxgw/LxgwWenKai)

### 1.2 工具

- fontTools - [子集化功能 pyftsubset](https://fonttools.readthedocs.io/en/latest/subset/)

- 夜煞之乐2001(NightFurySL2001) - [字体计数软件 CJK-character-count](https://github.com/NightFurySL2001/CJK-character-count)

### 1.3 语料

- 《通用规范汉字表》一级字

- 《信息交换用汉字编码字符集 基本集》第一级汉字

- 《义务教育语文课程常用字表》

- 《现代汉语常用字表》

- 《现代汉语常用词表》

- [《现代汉语语料库词频表》](http://corpus.china-language.edu.cn/Resources.aspx#LinkButton3)

- 《普通话水平测试用普通话词语表》表一、表二

- [清华大学开放中文词库](https://github.com/thunlp/THUOCL)

  注：

- 《现代汉语语料库词频表》内含“一九八０”词条，疑似有误，已替换成“一九八〇”；

- 《现代汉语常用词表》、清华大学开放中文词库等内含的非汉字字符已剔除。



## 2 文件

```
### 2.1 字体文件列表

/* TTF 格式 */
/ttf/lxgw-wenkai.original.v1.110-21.10.14.ttf
/ttf/lxgw-wenkai.subset.6801.char.ttf
/ttf/lxgw-wenkai.subset.6801.char.symbol.ttf

/* WOFF2 格式 */
/woff2/lxgw-wenkai.original.v1.110-21.10.14.woff2
/woff2/lxgw-wenkai.subset.6801.char.woff2
/woff2/lxgw-wenkai.subset.6801.char.symbol.woff2

/* 语料 */
位于 /corpus/ 目录下


### 2.2 说明

文件名含 original 的是 @落霞孤鹜 发布的未子集化的源文件，
版本号 v1.110-21.10.14

文件名含 subset 的是子集化后的文件，
汉字数量 6801，为上述数份语料的并集，基本囊括了常见汉字

其中：
  char 仅包含汉字
  char.symbol 包含汉字与常用符号

本子集化字体不含拉丁字母与阿拉伯数字


### 2.3 使用

若您要使用 WebFont，那么在上述列表中需要用到的文件前
添加 https://cdn.jsdelivr.net/npm/lxgw-wenkai-subset@latest 
即可使用 jsDelivr 的 CDN 全球加速服务，

例如：

https://cdn.jsdelivr.net/npm/lxgw-wenkai-subset@0.4.0/woff2/lxgw-wenkai.subset.6801.char.symbol.woff2

建议使用 WOFF2 格式
```



## 其他

版本 0.4.0

npm 地址 https://www.npmjs.com/package/lxgw-wenkai-subset
