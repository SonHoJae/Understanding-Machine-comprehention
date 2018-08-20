# Understanding-Machine-comprehention

In this repository, I would like to summarize couple papers to understand [Bi-directional Attention Flow for Machine Comprehension](https://arxiv.org/abs/1611.01603).
## 1. Understanding Attention mechanism with [Neural Machine Translation by Jointly Learning to Align and Translate_ 2014](https://arxiv.org/abs/1409.0473)
> Prior to this paper, neural machine translation(nmt) has been focused with statistical machine translation(smt). this paper proposed a building nmt without phase to phase segmentation or toknization. Additionally, it resolved issue that Encoder-Decoder Model has "fixed-length vector" which can mislead variable-length input sentence. [1]
> In this paper, the model gets rid of RNN architecture to

[1] Although most of the previous works used to encode a variable-length input sentence into a fixed-length vector, it is not necessary, and even it may be beneficial to have a variable-length vector, as we will show later (NEURAL MACHINE TRANSLATION BY JOINTLY LEARNING TO ALIGN AND TRANSLATE)
