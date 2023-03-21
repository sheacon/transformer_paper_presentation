# Attention Is All You Need

## Paper
A. Vaswani et al., “[Attention Is All You Need](https://arxiv.org/abs/1706.03762)”, (2017).

## Talk Outline
- Review of Transformer Purpose and Architecture
- Compare with RNNs
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

### Architecture

Transformers are a neural network with several key components:
- Multi-head self-attention mechanism
- Positional encoding
- Feed-forward networks

<img width="394" alt="architecture" src="https://user-images.githubusercontent.com/89158603/226610537-eab94686-7c80-4a7d-903d-e4e65f0860d9.png">


## Code Demonstration of Classification Task
- Compare accuracy performance and computation cost

## Results

![performance](https://user-images.githubusercontent.com/89158603/226527782-86d9b5b8-2865-4f33-803e-a1e4c2a5cffd.png)

## Discussion Questions
- How does self-attention help the model better understand and process the input text?
- How does the attention mechanism in the Transformer architecture differ from other techniques like recurrent neural networks (RNNs)?

## Critical Analysis
- A thorough analysis of computational cost at inference time

## Resource Links
- [GloVe](https://nlp.stanford.edu/projects/glove/)
- [MoE](https://arxiv.org/abs/1701.06538)
- Subsequent models and improvements
- [Presentation video](https://learning.oreilly.com/videos/natural-language-processing/0636920373605/0636920373605-video329383/)

