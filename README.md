# Understanding-Machine-comprehention

In this repository, I would like to summarize couple papers to understand [Bi-directional Attention Flow for Machine Comprehension](https://arxiv.org/abs/1611.01603).
## 1. Understanding "Attention mechanism" with [Neural Machine Translation by Jointly Learning to Align and Translate_ 2014](https://arxiv.org/abs/1409.0473)

### (1) Motivation
#### It's not possible to convey sentence to another with fixed-vector instead, it suggests to search particular hidden states to influence translation parts
> Prior to this paper, neural machine translation(nmt) has been focused with statistical machine translation(smt). this paper proposed a building nmt without phase to phase segmentation or toknization. Additionally, it resolved issue that Encoder-Decoder Model has "fixed-length vector" which can mislead variable-length input sentence. [1]

![Learning To Align And Translate](https://image.slidesharecdn.com/summarizationforh2omeetup12sep2017final-170918200049/95/the-magic-of-text-summarization-using-deep-networks-9-638.jpg?cb=1513351713 "Learning To Align And Translate")

### (2) Idea
#### DECODER: GENERAL DESCRIPTION
> By building attention network, it gets rid of fixed-vector and find annotations surrounding a specific input source
#### ENCODER: BIDIRECTIONAL RNN FOR ANNOTATING SEQUENCES
> The usual RNN, described in Eq. (1), reads an input sequence x in order starting from the first
symbol x1 to the last one xTx . However, in the proposed scheme, we would like the annotation
of each word to summarize not only the preceding words, but also the following words. Hence,
we propose to use a bidirectional RNN (BiRNN, Schuster and Paliwal, 1997), which has been
successfully used recently in speech recognition (see, e.g., Graves et al., 2013).

### Reference
[1] Although most of the previous works used to encode a variable-length input sentence into a fixed-length vector, it is not necessary, and even it may be beneficial to have a variable-length vector, as we will show later (NEURAL MACHINE TRANSLATION BY JOINTLY LEARNING TO ALIGN AND TRANSLATE)

<hr/>
