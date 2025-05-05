# 🧠 Large Language Model From scratch with PyTorch

This project implements a simple transformer-based language model using PyTorch. It includes training, evaluation, and text generation from a prompt.

---

## 🚀 Features

- Minimal GPT-like architecture
- Token-based text generation
- Training with AdamW optimizer
- Loss evaluation on training and validation sets
- Custom tokenizer (encode/decode functions)
- Text generation from custom prompts

---

## 📁 Files

- `myllm.ipynb`: Main Jupyter notebook containing the model implementation, training loop, and generation code.

---

## 📦 Requirements

- Python 3.8+
- PyTorch
- NumPy

You can install the dependencies using:

```bash
pip install torch numpy
```
🏃‍♂️ How to Run
Open myllm.ipynb in Jupyter Notebook or VSCode.

Run the cells sequentially to:

Train the model

Evaluate losses

Generate text using a prompt
```python
prompt = 'Hello! Can you see me?'
context = torch.tensor(encode(prompt), dtype=torch.long, device=device)
generated = decode(m.generate(context.unsqueeze(0), max_new_tokens=100)[0].tolist())
print(generated)
```
