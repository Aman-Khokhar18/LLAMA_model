Download the weights from: [https://github.com/facebookresearch/l...](https://github.com/meta-llama/llama)


---

# 🦙 LLaMA: Large Language Model from Scratch in PyTorch

This repository provides a clean and educational implementation of the **LLaMA** (Large Language Model Meta AI) transformer model entirely from scratch using **PyTorch**. It supports loading the official Meta model weights, performing inference (text completion), and understanding the inner workings of transformer blocks.

📽️ You can also view the **slides** in `presentation.pdf` to get a visual explanation of how the model works step-by-step.

---

## 🚀 Features

- Pure PyTorch implementation (no external transformer libraries)
- Full LLaMA model pipeline with:
  - Tokenizer loading
  - Model weight loading
  - Rotary positional embeddings
  - Self-attention and feedforward layers
  - Top-p sampling for generation
- Supports LLaMA 2 model sizes: 7B, 13B, 70B (chat and base)
- Inference with text prompts and prompt batching
- Highly modular design for educational purposes

---

## 📂 Project Structure

```

.
├── download.sh                  # Script to download LLaMA 2 model weights and tokenizer
├── model.py                    # Model definitions (Transformer, Attention, etc.)
├── run\_llama.py                # Loads model, tokenizer, runs inference
├── presentation.pdf            # Slides explaining the model architecture
├── tokenizer.model             # Tokenizer model (downloaded)
├── llama-2-7b/                 # Folder where weights are stored (example: 7B model)
└── README.md                   # You're here!

````


## 📥 Setup

### 1. Clone the repository
```bash
git clone https://github.com/your-username/llama-from-scratch
cd llama-from-scratch
````

### 2. Download model weights

Run the provided `download.sh` script:

```bash
bash download.sh
```

You will be prompted to paste the **presigned URL** from Meta (sent via email after acceptance of license) and choose the model(s) to download.

---

## 🧠 Run Inference

Run the following script to load the model and generate text completions:

```bash
python run_llama.py
```

The script includes several sample prompts, including few-shot and zero-shot examples.

---

## 🛠 Requirements

* Python 3.8+
* PyTorch (CPU or GPU)
* `tqdm`, `sentencepiece`

Install dependencies:

```bash
pip install torch tqdm sentencepiece
```

---

## 📚 Learn More

Want to understand how the architecture works? Open the `presentation.pdf` file included in this repo to view detailed slides explaining:

* Rotary embeddings
* Self-attention
* KV cache reuse
* Model block structure
* Top-p sampling for generation

---

## 📜 License

This code is licensed under the **LLaMA 2 Community License Agreement**. Please see `LICENSE` and `USE_POLICY.md` for more information.

---

## 🙌 Acknowledgements

* Meta AI for releasing LLaMA 2 and weights
* Original research paper: [https://arxiv.org/abs/2307.09288](https://arxiv.org/abs/2307.09288)

---

Feel free to fork, explore, and modify. Contributions and feedback are welcome!

```

---

Let me know if you'd like me to add badges (e.g., Python version, license) or generate this file programmatically in a `.md` file for you.
```
