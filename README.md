# TextRank-Extractive-Summary

参考文章：[基于TextRank算法的文本摘要（附Python代码）](https://www.jiqizhixin.com/articles/2018-12-28-18)

原文以同领域多篇文章输入，生成的一个单要点摘要。本项目以独立整篇文章作为输入，分别输出每篇文章的摘要。

目录结构：

```
.
├── SentenceSplit.py
├── __pycache__
│   └── SentenceSplit.cpython-37.pyc
├── sample_article.txt
├── sgns.wiki.word
├── sgns.wiki.word.bz2
├── stop_words.txt
└── summary_chinese.ipynb
```

- ```SentenceSplit.py```参考于用户@GLZ1925给出的[中文分句方法](https://github.com/GLZ1925/-)
- ```sample_article.txt```随机取自[雷锋网](https://www.leiphone.com/)最新文章
- ```sgns.wiki.word.bz2```为[Chinese Word Vectors 中文词向量](https://github.com/Embedding/Chinese-Word-Vectors)中的[Wikipedia_zh 中文维基百科](https://pan.baidu.com/s/1AmXYWVgkxrG4GokevPtNgA)预训练模型。解压后得到```sgns.wiki.word```，使用时请删除文档中第一行数据形状信息。
- ```stop_words.txt```中文停用词
- ```summary_chinese.ipynb```TextRank算法实现代码
