# 洛克生词本
这个应用可以帮助你识别一篇文字中你不认识的那些单词，并给出发音、解释和例句。
工作原理是，识别每个单词的原型，并过滤掉你在myvocab文件中已输入的单词。
当然，你也可以指定只查找某些单词。

最开始的目的是作者希望导入这样的形式到Anki中学习，
当然，你也可以把生成的词表，用“不背单词”app的自定义词书功能，导入这些单词进行学习。


网页版：
    http://www.pengci.co

本地版环境要求：

    请使用python3.7环境（如果你是之前的用户，请卸载python2.7或升级到python3.7)。

内含文件介绍：

    freq_list文件是一个精心挑选的词频列表，一般来说越靠前的词越简单
    myvocab文件是你“已经熟悉”的单词，默认只添加了简单的星期词和示例简单词

> 建议你根据freq_list筛选出一份你已经熟悉的单词，把这些熟悉的单词放到myvocab文件中
    
    
    底层实现使用了stardict.py和startdict.db，以及lemma.en.txt，是使用的skywind3000的开源词典：
    https://github.com/skywind3000/ECDICT
