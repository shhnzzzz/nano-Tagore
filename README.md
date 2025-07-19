# nanoTagore   
This project trains a GPT-style character-level language model on the poems and songs of Rabindranath Tagore, inspired by [Andrej Karpathy's nanoGPT](https://github.com/karpathy/nanoGPT). Our goal is to generate Tagore-style poetry using a minimal transformer-based architecture.


## Key Features 

Train a GPT-style Language Model on Rabindranath Tagore’s Works.
Built upon Andrej Karpathy’s NanoGPT, this project retains a clean and modular codebase ideal for understanding, experimentation, and customization.The architecture and config system make it easy to modify datasets, model size, training procedures, or sampling strategies for rapid iteration and research.

# Model Architecture 

This project implements a GPT-style decoder-only Transformer, adapted for training on Rabindranath Tagore’s poetic works.

The model follows a decoder-only Transformer architecture similar to GPT-2. It consists of:

    Token & Positional Embeddings

    Stack of Transformer Blocks (12 layers by default), each with:

        Multi-head self-attention

        Feedforward network

        Layer normalization and residual connections

    Final Linear Layer projecting to vocabulary logits

The architecture is fully autoregressive and trained with causal masking, enabling it to generate text one token at a time.

# Generate Poems with our trained model
This project already includes a pretrained GPT model on Rabindranath Tagore's poetry. You can generate poems instantly without retraining.

 **Open the colab notebook** - [Poem Generator](https://colab.research.google.com/drive/1v9u1bhSiwpGdul3WhpK8yy402JgjR0S-?usp=sharing)
 
<details>
  <summary><strong> Run all cells</strong></summary>

  - Automatically download the pretrained model (ckpt.pt)
  - Load it using sample.py
  - Generate beautiful poems in the style of Tagore


</details>



