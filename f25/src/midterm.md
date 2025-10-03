# Midterm Exam Topics (75 minutes)

## Question 1: Probability & Language Modeling (20 minutes)
**Topics from L3:**
- N-gram language models: Chain rule, Markov assumption, MLE estimation
- Smoothing techniques: Laplace smoothing, backoff methods
- Perplexity calculation: PP(W) = (P(w₁...wₙ))^(-1/n)
- Mathematical derivations: Conditional probabilities, chain rule applications

**Sample problems:**
- Calculate bigram probabilities from a corpus
- Apply Laplace smoothing to handle unseen n-grams
- Compute perplexity for a given sequence
- Derive MLE for n-gram parameters

## Question 2: Neural Networks & Recurrent Architectures (20 minutes)
**Topics from L4-L5, L7:**
- MLP architecture: Forward pass, activation functions (sigmoid, ReLU, tanh)
- Backpropagation algorithm: Chain rule, gradient computation
- RNN architecture: Hidden states, sequential processing, h_t = σ(W_h h_{t-1} + W_x x_t + b)
- LSTM gates: Forget, input, output gates; cell state management
- Training dynamics: BPTT, vanishing/exploding gradients, gradient clipping
- Loss functions: Cross-entropy for classification, MSE for regression

**Sample problems:**
- Compute forward pass through a 2-layer MLP
- Derive gradients using chain rule for RNNs (BPTT)
- Implement LSTM gate computations
- Analyze vanishing gradient problem in RNNs vs solutions
- Compare RNN vs MLP for sequential data

## Question 3: Attention & Transformers (20 minutes)
**Topics from L8-L9:**
- Attention mechanism: Query-Key-Value framework, scaled dot-product attention
- Transformer architecture: Encoder-decoder structure, multi-head attention
- Mathematical formulations: Attention(Q,K,V) = softmax(QK^T/√d_k)V
- Positional encoding: Sinusoidal encoding, why it works

**Sample problems:**
- Compute attention weights for a given sequence
- Explain the difference between self-attention and cross-attention
- Derive the scaling factor √d_k in attention
- Compare RNNs vs Transformers for sequence modeling

## Question 4: GPT Evolution, Alignment & Reinforcement Learning (15 minutes)
**Topics from L10-L12:**
- GPT progression: GPT-1 (transfer learning) → GPT-2 (zero-shot) → GPT-3 (in-context learning)
- Alignment techniques: SFT vs RLHF, Bradley-Terry model for preferences
- RL fundamentals: MDP formulation, value functions, policy optimization
- RLHF as contextual bandit: Context (prompt), Action (response), Reward (preference)
- Mathematical formulations: L_SFT, L_RM, L_PPO objectives
- Key insights: Scale enables capabilities, alignment shapes behavior

**Sample problems:**
- Compare supervised learning vs imitation learning vs preference learning
- Explain the three-stage training pipeline (pretraining → SFT → RLHF)
- Derive the Bradley-Terry preference model
- Map RLHF to MDP/bandit framework
- Analyze why RLHF is needed beyond SFT

## Question Distribution & Timing:
- Q1 (20 min): Probability foundations - computational and derivations
- Q2 (20 min): Neural networks - mathematical and implementation
- Q3 (20 min): Attention/Transformers - conceptual and mathematical
- Q4 (15 min): GPT/Alignment - conceptual understanding and connections

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
**Format: 4 questions, mixed computational and conceptual**
