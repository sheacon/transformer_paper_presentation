# Attention Is All You Need

## Paper
A. Vaswani et al., “[Attention Is All You Need](https://arxiv.org/abs/1706.03762)”, (2017).

## Talk Outline
- Review paper
- Review prior NLP approaches
- Compare application to classification task

## Paper Overview

Transformers are a neural network architecture introduced by Vaswani et al. (2017) for natural language processing tasks. Key components of the architecture include:
- Multi-head self-attention mechanism: Computes attention scores for input tokens, capturing dependencies irrespective of their positions in the sequence.
- Positional encoding: Injects positional information into input embeddings to retain sequence order information.
- Layer normalization: Stabilizes training by normalizing layer outputs.
- Feed-forward networks: Consist of fully connected layers applied after the multi-head self-attention mechanism.
- Residual connections: Allow gradients to flow more effectively, preventing vanishing gradient issues.

Transformers typically have an encoder-decoder structure for tasks like machine translation, or use only the encoder for tasks like text classification and sentiment analysis.

### Architecture

## NLP Previous Approaches

Transformers addressed several problems in previous NLP approaches:
- Long-range dependencies: The self-attention mechanism captures dependencies between tokens, regardless of their distance, overcoming limitations of RNNs and LSTMs in learning long-range dependencies.
- Parallelization: Transformers process input sequences in parallel, enabling faster training compared to sequential processing in RNNs and LSTMs.
- Scalability: Transformers can scale to large amounts of data and have enabled the development of large pre-trained models like GPT and BERT, which significantly improved performance across various NLP tasks.
- Transfer learning: Pre-trained Transformer models can be fine-tuned for specific tasks, leading to better performance with less labeled data compared to traditional methods.
- Contextualized word representations: Unlike context-independent embeddings (e.g., Word2Vec and GloVe), Transformers generate context-aware representations, capturing nuances in word meanings based on their usage in a sentence.

These improvements have led to the widespread adoption of Transformer models in NLP and their superior performance on a variety of tasks.

### Word2Vec and GloVe

Word2Vec and GloVe are popular unsupervised learning algorithms for generating dense word embeddings. Word2Vec, based on neural networks, captures semantic and syntactic relationships by predicting context words given a target word. GloVe, short for Global Vectors, constructs co-occurrence matrices to capture word relationships, combining global and local context information. Both methods produce semantically meaningful vector representations for words.

Transformers are attention-based neural architectures for NLP tasks, processing input sequences in parallel, whereas Word2Vec and GloVe generate word embeddings only.

### RNN

Recurrent Neural Networks (RNNs), including Long Short-Term Memory (LSTM) and Gated Recurrent Unit (GRU) variants, are sequential models that process input data through hidden states, allowing them to capture temporal dependencies. They dominated NLP before Transformers, which addressed RNNs' limitations, such as difficulty in learning long-range dependencies and lack of parallelism.

Transformers use self-attention mechanisms for parallel processing and effectively learn long-range dependencies, overcoming RNNs' sequential limitations and computational inefficiencies.

## Code Demonstration of Classification Task
- Compare accuracy performance and computation cost

## Discussion Questions
- Question 1
- Question 2

## Critical Analysis

## Resource Links
- Paper itself again
- Word2Vec/GloVe papers/tools
- RNN papers/tools
- Subsequent models and improvements
- [Presentation video](https://learning.oreilly.com/videos/natural-language-processing/0636920373605/0636920373605-video329383/)

