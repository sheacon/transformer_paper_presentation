# Attention Is All You Need

## Paper
A. Vaswani et al., “[Attention Is All You Need](https://arxiv.org/abs/1706.03762)”, (2017).

## Talk Outline
- Review of Transformer Purpose and Architecture
- Compare with RNNs and CNNs
- Assess Results
- Question Attention with Use Case

## Why Transformer?
- Problem: Sequence Transduction (e.g. Machine Translation)
- Existing Approach Limitations
  - Context-Independent Embeddings (Word2Vec and GloVe)
  - RNN and CNN (Performance and Training)
    - Long-Range Dependencies
    - Parallelization
    - Limited Transfer Learning

![complexity](https://user-images.githubusercontent.com/89158603/226613881-f4542702-38ae-49ec-8bce-7eb4d804ccb0.png)

### Architecture

Transformers are a neural network with several key components:
- Encoder and decoder stacks
- Multi-head self-attention mechanism
- Positional encoding
- Feed-forward networks

<img width="394" alt="architecture" src="https://user-images.githubusercontent.com/89158603/226613542-85068176-a82f-4f5a-9458-cf438f00dc15.png">

## Results

![params](https://user-images.githubusercontent.com/89158603/226614603-7c6fb4a5-067c-4edd-ad5f-d979ad42f7a4.png)

![performance](https://user-images.githubusercontent.com/89158603/226613498-b3b7177d-1516-434f-8051-026bb973aa67.png)
(bilingual evaluation understudy)

## Discussion Questions
- How does self-attention help the model better understand and process the input text?
- How does the attention mechanism in the Transformer architecture differ from other techniques like recurrent neural networks (RNNs)?

## Look Ma', No Attention
- Do we always need attention?
[Classification Task Notebook]()

## Critical Analysis
- More thorough discussion of computational cost at inference time

## Resource Links
- [GloVe](https://nlp.stanford.edu/projects/glove/)
- [Recurrent Neural Networs](https://en.wikipedia.org/wiki/Recurrent_neural_network)
- [MoE](https://arxiv.org/abs/1701.06538)
- [BLEU](https://en.wikipedia.org/wiki/BLEU)
- [Presentation video](https://learning.oreilly.com/videos/natural-language-processing/0636920373605/0636920373605-video329383/)

