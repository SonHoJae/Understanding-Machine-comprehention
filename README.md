# Understanding-Machine-comprehention

In this repository, I would like to summarize couple papers to understand 
[Bi-directional Attention Flow for Machine Comprehension](https://arxiv.org/abs/1611.01603).
## 1. Understanding "Attention mechanism" with [Neural Machine Translation by Jointly Learning to Align and Translate_2014](https://arxiv.org/abs/1409.0473)

### (1) Motivation
#### It's not possible to convey sentence weights to target with fixed-vector instead, it suggests to search particular hidden states to influence translation parts
> Prior to this paper, neural machine translation(nmt) has been focused with statistical machine translation(smt). this paper proposed a building nmt without phase to phase segmentation or toknization. Additionally, it resolved issue that Encoder-Decoder Model has "fixed-length vector" which can mislead variable-length input sentence. The jounal says "Although most of the previous works used to encode a variable-length input sentence into a fixed-length vector, it is not necessary, and even it may be beneficial to have a variable-length vector, as we will show later"

![Learning To Align And Translate](https://image.slidesharecdn.com/summarizationforh2omeetup12sep2017final-170918200049/95/the-magic-of-text-summarization-using-deep-networks-9-638.jpg?cb=1513351713 "Learning To Align And Translate")

### (2) Idea
#### DECODER: GENERAL DESCRIPTION
> By building attention network, it gets rid of fixed-vector and find annotations surrounding a specific input source
#### ENCODER: BIDIRECTIONAL RNN FOR ANNOTATING SEQUENCES
> The jounal says "The usual RNN, described in Eq. (1), reads an input sequence x in order starting from the first
symbol x1 to the last one xTx . However, in the proposed scheme, we would like the annotation
of each word to summarize not only the preceding words, but also the following words. Hence,
we propose to use a bidirectional RNN (BiRNN, Schuster and Paliwal, 1997), which has been
successfully used recently in speech recognition (see, e.g., Graves et al., 2013)."

### Reference
[1]  (NEURAL MACHINE TRANSLATION BY JOINTLY LEARNING TO ALIGN AND TRANSLATE)

<hr/>

## 2. Reading comprehension style question answering with [R-NET: MACHINE READING COMPREHENSION WITH SELF-MATCHING NETWORKS_2017](https://www.microsoft.com/en-us/research/publication/mrc/)

## Reference
> 1. [Bi-directional Attention Flow for Machine Comprehension](https://arxiv.org/abs/1611.01603)
> 2. [Learning To Align And Translate](https://image.slidesharecdn.com/summarizationforh2omeetup12sep2017final-170918200049/95/the-magic-of-text-summarization-using-deep-networks-9-638.jpg?cb=1513351713 "Learning To Align And Translate")
> 3. [R-NET: MACHINE READING COMPREHENSION WITH SELF-MATCHING NETWORKS_2017](https://www.microsoft.com/en-us/research/publication/mrc/)
> 4. [Understanding R-Net: Microsoft’s ‘superhuman’ reading AI](https://codeburst.io/understanding-r-net-microsofts-superhuman-reading-ai-23ff7ededd96)
> 5. [NMT Concepts and Parameters_sendtex_Youtube](https://www.youtube.com/watch?v=gFxiQXnt9w4)
> 6. [CS224D_Lecture 16: Dynamic Neural Networks for Question Answering](https://www.youtube.com/watch?v=T3octNTE7Is)
> 7. [Challenges of reproducing R-NET neural network using Keras](http://yerevann.github.io/2017/08/25/challenges-of-reproducing-r-net-neural-network-using-keras/)
> 8. [CS224D_Lecture 9: Machine Translation and Advanced Recurrent LSTMs and GRUs](https://www.youtube.com/watch?v=QuELiw8tbx8&list=PL3FW7Lu3i5Jsnh1rnUwq_TcylNr7EkRe6&index=10&t=0s)
> 9. [CS224D_Lecture 3 | GloVe: Global Vectors for Word Representation](https://www.youtube.com/watch?v=ASn7ExxLZws&index=3&list=PL3FW7Lu3i5Jsnh1rnUwq_TcylNr7EkRe6)
