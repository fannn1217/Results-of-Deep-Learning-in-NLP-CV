## Pre-train

* **ULMFiT** “Universal Language Model Fine-tuning for Text Classification” **ACL(2018)**
  [[paper](https://arxiv.org/abs/1801.06146)]
  [[code](http://nlp.fast.ai/ulmfit)]
  [[reading note](https://www.jianshu.com/p/5b680f4fb2f2)]
  
  
* **GPT**  “Improving Language Understanding by Generative Pre-Training” **（2018）**
  [[paper](https://s3-us-west-2.amazonaws.com/openai-assets/research-covers/language-unsupervised/language_understanding_paper.pdf)]
  [[github](https://github.com/openai/finetune-transformer-lm)]
  [[guide](https://finetune.indico.io/#)]
  
标注数据稀少，对无标记的数据进行pre-train是一种提高模型效果的方法。本文使用transformer（decoder only）在无标记语料上进行预训练language model，之后经过模型的fine-tuning，实现对QA，语义相似度，分类等任务的效果提升。
  
* **BERT**  “BERT: Pre-training of Deep Bidirectional Transformers for Language Understanding” **（2018）**
  [[paper](https://arxiv.org/abs/1810.04805)]
  [[github](https://github.com/google-research/language)]
  [[reading note](https://www.jiqizhixin.com/articles/2018-10-12-13)]
  
不同于GPT等方法（预训练语言模型后微调），本文使用多层双向 Transformer 编码器，不使用传统的从左到右或从右到左的语言模型来预训练 BERT，而是使用两个新型无监督预测任务来进行预训练。这两个新任务分别是Masked LM 和下一句预测。实验表明，BERT 刷新了 11 项 NLP 任务的当前最优性能记录。

* **Probing Tasks**  “Linguistic Knowledge and Transferability of Contextual Representations” **NAACL（2019）**
  [[paper](https://arxiv.org/abs/1903.08855)]
  [[github](https://github.com/nelson-liu/contextual-repr-analysis)]
  [[reading note](https://zhuanlan.zhihu.com/p/62462743)]
  
Probing Tasks类的论文，对于当前流行的预训练词向量CWRs成果进行了比较探索，，如ELMo，OpenAI的transformer语言模型和BERT。

本文研究以下几个问题：

1、这些表示向量捕获了哪些语言特征？

2、在contextualizers中，每层的可迁移性为何不同？

3、预训练任务的选择如何影响向量的学习？

* **TALK** “预训练语言模型研究进展和趋势展望”, an invited talk at **全国计算语言学大会（CCL2020）**
  [[link](https://liuquncn.github.io/talks/20201031-CCL/pre-trained-langauge-models-research-advances-and-prospectives.pdf)]
  [[author](https://liuquncn.github.io/)]
