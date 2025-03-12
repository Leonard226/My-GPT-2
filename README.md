# **GPT-2 From Scratch**
This repo is a simple inference implementation of GPT-2 using its tokenizer and learned weights. It is based on this blog post: [GPT-2 From Scratch](https://jaykmody.com/blog/gpt-from-scratch/).  

It implements the transformer architecture of GPT-2, extracting **token embeddings** with **positional encodings**, and constructing the **transformer blocks** that include **Multi-Headed Attention** and a **Feed-Forward Network (MLP)**, all using the original **GPT-2 hyperparameters**.

## **Usage**
To generate text, simply call:

```python
from my_gpt2 import main

output = main(prompt="How are you doing?", n_tokens_to_generate=40, model_size="124M", models_dir="models")
print(output)
```

## **Implementation Details**
For a detailed explanation of the model, refer to **`my_gpt2.ipynb`**, where all core components (token embedding, self-attention, transformer blocks, residual connections, etc.) are explained and demonstrated.
