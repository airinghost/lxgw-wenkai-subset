
## 致谢 Acknowledgments

- 落霞孤鹜(LXGW) - [霞鹜文楷 LXGW WenKai](https://github.com/lxgw/LxgwWenKai)

- fontTools - [子集化功能 pyftsubset](https://fonttools.readthedocs.io/en/latest/subset/)

- 夜煞之乐2001(NightFurySL2001) - [字体计数软件 CJK-character-count](https://github.com/NightFurySL2001/CJK-character-count)



## 语料 Corpus

- 《通用规范汉字表》一级字、二级字

- 《信息交换用汉字编码字符集 基本集》第一级汉字

- 《义务教育语文课程常用字表》

- 《现代汉语常用字表》

- [《现代汉语语料库词频表》](http://corpus.china-language.edu.cn//Resources.aspx#LinkButton3)



## 文件 Files

```
### 列表

/* TTF files */
/ttf/lxgw-wenkai.original.v1.110-21.10.14.ttf
/ttf/lxgw-wenkai.subset.6507.char.ttf
/ttf/lxgw-wenkai.subset.6507.char.symbol.ttf
/ttf/lxgw-wenkai.subset.6507.char.symbol.num.ttf
/ttf/lxgw-wenkai.subset.6507.char.symbol.latin.ttf
/ttf/lxgw-wenkai.subset.6507.char.symbol.num.latin.ttf

/* WOFF2 files */
/woff2/lxgw-wenkai.subset.6507.char.woff2
/woff2/lxgw-wenkai.subset.6507.char.symbol.woff2
/woff2/lxgw-wenkai.subset.6507.char.symbol.num.woff2
/woff2/lxgw-wenkai.subset.6507.char.symbol.latin.woff2
/woff2/lxgw-wenkai.subset.6507.char.symbol.num.latin.woff2

/* Corpus */
/corpus/corpus.6507.char.txt
/corpus/corpus.6507.char.symbol.txt
/corpus/corpus.6507.char.symbol.num.txt
/corpus/corpus.6507.char.symbol.latin.txt
/corpus/corpus.6507.char.symbol.num.latin.txt


### 说明

文件名含 original 的是落霞孤鹜发布的未子集化的源文件，版本号 v1.110-21.10.14

文件名含 subset 的是子集化后的文件，汉字数量 6507，为五份语料的并集，基本囊括了常见汉字。其中：
  char 仅包含汉字
  char.symbol 包含汉字与常用符号
  char.symbol.num 包含汉字、常用符号以及数字
  char.symbol.latin 包含汉字、常用符号以及拉丁字母
  char.symbol.num.latin 包含汉字、常用符号、数字以及拉丁字母


### 使用

若您要使用 WebFont，那么在上述列表中需要用到的文件前添加 https://cdn.jsdelivr.net/npm/lxgw-wenkai-subset@0.3.0 即可使用 jsDelivr 的 CDN 全球加速服务。建议使用 WOFF2 格式。
```



## 其他 P.S.

版本 0.1.x 至 0.2.x 缺了一些常见字（虽然这些字不一定常用）。

Version 0.1.x-0.2.x lack some common (but may not be frequently used) characters.
