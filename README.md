# Historical Project Mod - Chinese Localization

[项目概览 - Historical Project Mod - ParaTranz](https://paratranz.cn/projects/4254)

### 从ParaTranz导出翻译结果后在gbk字符集下特殊符号的处理

csv文件中存在一些特殊符号，即§R, §G, §B, §Y, §!, ¤。如果用gbk字符集打开csv文件后，§就会变成搂，¤会变成陇。

只要在iso8859-1字符集下将特定的字符换成§和¤即可，一种简单的处理方法如下：

1. 在gbk字符集下打开csv文件，将“搂”和“陇”转成文本中没有的**【英文】**字符，保存
2. 然后用iso8859-1字符集打开同个文件，将**【英文】**字符转成§或¤，保存

这样在游戏中就能正常改变字体颜色和显示金钱￡符号了
