# point-generator 论文读书笔记
## introduce
* RNN用于生成摘要存在的缺陷：不能准确地复制事实细节，无法处理词汇不足（OOV）单词，并容易造成重复。
* 这篇论文通过指针生成网络提高了精确性和处理OOV词的能力，并且保留了生成新词的能力。
* 针对重复，该论文提出了汇聚机制(coverage machine),跟踪和控制目前被覆盖的单词。
## model
* sequence-to-sequence(baseline)
![seq2seq](https://img-blog.csdnimg.cn/20190604141751164.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L21yMnpoYW5n,size_16,color_FFFFFF,t_70)
