# Attention Is All You Need

## Paper
A. Vaswani et al., “[Attention Is All You Need](https://arxiv.org/abs/1706.03762)”, (2017).

## Talk Outline
- Review of Purpose and Architecture of Transformer Models
- Compare with RNNs and CNNs
- Assess Results
- Business Use Case / Costs

## Why The Transformer?
- Problem: Sequence Transduction (e.g. Language Translation)
- Approach Novelty: Self-Attention Mechanism

![performance](https://user-images.githubusercontent.com/89158603/226637249-19c6d3ba-deb8-455d-a773-47df5cd3b8a6.png)

- Existing Approach Limitations
  - RNN and CNN (Performance and Training)
    - Limited Long-Range Dependencies
    - Difficult Parallel Computation (RNN)

![RNN](https://user-images.githubusercontent.com/89158603/226617472-66e77c79-bbcf-4b3e-b0cd-522106c11fc5.png)

![CNN](https://user-images.githubusercontent.com/89158603/226622988-283456f3-a0af-4476-bfa2-deb9a8114da6.png)

![complexity3](https://user-images.githubusercontent.com/89158603/226626954-c7765888-9937-4045-9a38-b75754e820be.png)

### Architecture

Transformers are a neural network with several key components:
- Encoder and decoder stacks
- Multi-head self-attention mechanism
- Positional encoding
- Feed-forward networks

![encoder_decoder](https://user-images.githubusercontent.com/89158603/226618259-bf38f44d-e723-49a3-b978-d4a3c8fe2ad3.png)

#### Question 1: Why does the encoder-decoder structure make sense for translation?
- How do these two components work together?
- Encoder does what with input?
- Decoder does what with encoder output?

<img width="149" alt="architecture" src="https://user-images.githubusercontent.com/89158603/226651705-22af9028-3b20-4fe9-a27a-bc569e716b39.png">

![attention](https://user-images.githubusercontent.com/89158603/226624292-15fe76b2-02e0-49ae-a852-05bd6fd4d982.png)

#### Question 2: Does self-attention have computational downsides?
- How does efficiency change with sequence length?

![formal_algo](https://user-images.githubusercontent.com/89158603/226646079-610909d5-2688-4194-801c-13138fe98d6f.png)

(#### Optional Question: What is the benefit of multi-head attention over single-head?)
- Does each head do anything different?

## Results

![params](https://user-images.githubusercontent.com/89158603/226614603-7c6fb4a5-067c-4edd-ad5f-d979ad42f7a4.png)

![performance](https://user-images.githubusercontent.com/89158603/226613498-b3b7177d-1516-434f-8051-026bb973aa67.png)

(bilingual evaluation understudy)

## Business Case: Look Ma', No Attention
- Do we always need attention?
- Context-Independent Embeddings (Word2Vec and GloVe)
- [Classification Task Notebook](classification_task.ipynb)

## Critical Analysis
- More thorough discussion of computational cost at inference time

## Resource Links
- [GloVe](https://nlp.stanford.edu/projects/glove/)
- [Sequence to Sequence Learning (2014)](https://arxiv.org/abs/1409.3215)
- [Recurrent Neural Networs](https://en.wikipedia.org/wiki/Recurrent_neural_network)
- [MoE](https://arxiv.org/abs/1701.06538)
- [BLEU](https://en.wikipedia.org/wiki/BLEU)
- [Presentation video](https://learning.oreilly.com/videos/natural-language-processing/0636920373605/0636920373605-video329383/)
- [Formal Algorithms for Transformers](https://arxiv.org/abs/2207.09238)

