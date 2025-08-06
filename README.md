# 🔤 Character-Level Language Modeling: From Bigrams to Transformers

## 🧠 Project Goal

Our ultimate aim is to understand and build **Transformer-based models** for language modeling — the same foundation behind GPT and BERT. To truly appreciate their power, we’ve taken a bottom-up journey, starting with **the simplest models** and gradually adding complexity and capability.

---

## 🚀 Journey So Far

We began with a **bigram-based character-level language model** using a raw count matrix. This model taught us the limitations of pure frequency-based approaches:

- No generalization to unseen character pairs
- Cannot learn structure or adapt
- Generates nonsensical or highly repetitive text

To overcome these flaws, we implemented:

### ✅ 1. **Neural Bigram Model**
- A single-layer neural net with a 27×27 weight matrix
- Predicts the next character from a one-hot input
- **Limitations**: Still only looks one character back (no real sequence modeling)

### ✅ 2. **Feedforward Neural Network**
- Added hidden layers and non-linearities
- Improved generalization slightly
- **Still limited** by the lack of sequence awareness

### ✅ 3. **Recurrent Neural Network (RNN)**
- Introduced memory via hidden state
- Predicts next characters based on previous context
- Can learn spelling rules and character patterns
- Provides a solid base for understanding sequence modeling

---

## 📚 Why This Progression?

Before jumping into Transformers, it’s important to **understand what problems they solve**.

| Model        | Sequence Aware? | Learns from Context? | Handles Long-Term Dependencies? |
|--------------|------------------|-----------------------|----------------------------------|
| Bigram Count | ❌              | ❌                    | ❌                               |
| Neural Net   | ❌              | ✅ (slightly)         | ❌                               |
| RNN          | ✅              | ✅                    | ❌ (limited memory)             |
| Transformer  | ✅✅            | ✅✅                  | ✅✅✅                            |

> Each step in this project is designed to show **why Transformers are necessary**, not just how to use them.

---

## 🔍 What's Next?

We plan to implement:

- ✅ **LSTM**: Better memory management for long-term dependencies
- 🚧 **Transformer Encoder**: Multi-head attention and self-attention for global context
- 🚀 **Autoregressive Transformer**: Character-level generative model (GPT-style)

---

## 🧑‍💻 Technologies Used

- Python + PyTorch
- Matplotlib for visualization
- Kaggle notebooks (for experimentation)
- English word corpus (character-level)

---

## 📈 Metrics Tracked

- Training loss & test loss
- Generated sample quality
- Learning curve improvements


---

## 🙌 Acknowledgments

Inspired by Andrej Karpathy's [NanoGPT](https://github.com/karpathy/nanogpt) and the fundamental ideas behind GPT models.

---

## 📌 Final Thought

> To build strong models, you must understand weak ones.

This project is our foundational journey from basic statistics to cutting-edge sequence modeling — paving the way to truly grasp **how Transformers learn language**.
