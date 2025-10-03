# Midterm Exam Topics (75 minutes)

## 1: Probability & Language Modeling

**Topics from L3:**

- N-gram language models: Chain rule, Markov assumption, MLE estimation
- Smoothing techniques: Laplace smoothing, backoff methods
- Perplexity calculation: PP(W) = (P(w₁...wₙ))^(-1/n)
- Mathematical derivations: Conditional probabilities, chain rule applications

**Interview-style problems:**

- **System Design**: Design a text autocomplete system using n-gram models. How would you handle the cold start problem for new users?
- **Performance**: Your n-gram model has high perplexity on a new domain. What techniques would you use to adapt it?
- **Scalability**: How would you implement a trigram model that can handle 1M+ vocabulary size efficiently?
- **Evaluation**: Compare perplexity vs BLEU score for evaluating language models. When would you use each?

## 2: Neural Networks & Recurrent Architectures

**Topics from L4-L5, L7:**

- MLP architecture: Forward pass, activation functions (sigmoid, ReLU, tanh)
- Backpropagation algorithm: Chain rule, gradient computation
- RNN architecture: Hidden states, sequential processing, h*t = σ(W_h h*{t-1} + W_x x_t + b)
- LSTM gates: Forget, input, output gates; cell state management
- Training dynamics: BPTT, vanishing/exploding gradients, gradient clipping
- Loss functions: Cross-entropy for classification, MSE for regression

**Interview-style problems:**

- **Architecture Choice**: You're building a sentiment analysis system for social media. Would you use MLP, RNN, or LSTM? Justify your choice.
- **Debugging**: Your LSTM model's loss isn't decreasing. What are the top 3 things you'd check?
- **Production**: How would you optimize an RNN model for real-time inference with 100ms latency requirements?
- **Memory**: Your RNN is running out of memory on long sequences. What techniques would you use to handle this?
- **Gradient Issues**: Explain the vanishing gradient problem in RNNs and how you'd solve it in a production system.

## 3: Attention & Transformers

**Topics from L8-L9:**

- Attention mechanism: Query-Key-Value framework, scaled dot-product attention
- Transformer architecture: Encoder-decoder structure, multi-head attention
- Mathematical formulations: Attention(Q,K,V) = softmax(QK^T/√d_k)V
- Positional encoding: Sinusoidal encoding, why it works

**Interview-style problems:**

- **System Design**: Design a real-time translation system using transformers. How would you handle different input lengths and batch processing?
- **Performance**: Your transformer model is too slow for production. What optimization techniques would you implement?
- **Memory**: How would you handle very long sequences (10k+ tokens) with a transformer model?
- **Interpretability**: How would you visualize attention patterns to debug why your model is making wrong translations?
- **Scaling**: Your transformer model works well on 1M examples but poorly on 10M. What could be causing this and how would you fix it?

## 4: GPT Evolution, Alignment & Reinforcement Learning

**Topics from L10-L12:**

- GPT progression: GPT-1 (transfer learning) → GPT-2 (zero-shot) → GPT-3 (in-context learning)
- Alignment techniques: SFT vs RLHF, Bradley-Terry model for preferences
- RL fundamentals: MDP formulation, value functions, policy optimization
- RLHF as contextual bandit: Context (prompt), Action (response), Reward (preference)
- Mathematical formulations: L_SFT, L_RM, L_PPO objectives
- Key insights: Scale enables capabilities, alignment shapes behavior

**Interview-style problems:**

- **System Design**: Design a ChatGPT-like system from scratch. What are the key components and how would you scale it?
- **Alignment**: Your LLM is generating harmful content. How would you implement RLHF to fix this in production?
- **Evaluation**: How would you measure if your RLHF-trained model is actually more helpful than the base model?
- **Data**: You need to collect human preference data for RLHF. How would you design the data collection process?
- **Safety**: Your model is reward hacking (optimizing for the reward model instead of being helpful). How would you detect and fix this?
- **Scaling**: Your RLHF training is too expensive. What techniques would you use to make it more efficient?

## Question Distribution:

Q1-4: multiple choices
Q5-8: written answers

- Q1/Q5: Probability foundations - computational and derivations
- Q2/Q6: Neural networks - mathematical and implementation
- Q3/Q7: Attention/Transformers - conceptual and mathematical
- Q4/Q8: GPT/Alignment - conceptual understanding and connections

## Key Learning Objectives Tested:

1. Mathematical foundations: Probability, statistics, optimization
2. Neural network theory: MLP architecture, RNN/LSTM design, backpropagation
3. Modern architectures: Attention mechanisms, transformer design
4. AI alignment & RL: From capabilities to human-aligned systems via reinforcement learning

## Question Types:

- Computational: Calculate probabilities, gradients, attention weights
- Derivations: Mathematical proofs and formula derivations
- Conceptual: Explain mechanisms, compare approaches, analyze trade-offs
- Applications: Connect theory to real-world AI systems

## Coverage Summary:

This exam covers the core progression from statistical language models through neural networks (MLP, RNN, LSTM) to modern transformer architectures and AI alignment via reinforcement learning, testing both mathematical understanding and conceptual grasp of the field's evolution.

**Total Time: 75 minutes**
**Format: 8 questions, mixed computational and conceptual**
