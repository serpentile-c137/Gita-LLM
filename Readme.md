# Gita-LLM 🕉️📚🧠

**Gita-LLM** is an open-source project focused on fine-tuning large language models (LLMs) on the teachings and philosophy of the **Bhagavad Gita**, aiming to create a spiritual, therapeutic, and conversational AI grounded in ancient wisdom.

## 🌟 Project Vision

This project seeks to bridge the gap between ancient spiritual knowledge and modern AI by training LLMs to:
- Provide answers based on the Bhagavad Gita.
- Offer therapeutic, reflective, and philosophical responses.
- Support spiritual self-inquiry and emotional well-being.

## 📦 Resources

- 📚 **Dataset**: [`serpentilec137/gita-verse-qna-dataset`](https://huggingface.co/datasets/serpentilec137/gita-verse-qna-dataset)  
  A question-answer dataset inspired by verses from the Bhagavad Gita, curated for training and evaluation.

- 🤖 **Fine-tuned Model**: [`serpentilec137/gita-therapist-llm`](https://huggingface.co/serpentilec137/gita-therapist-llm)  
  A Mistral 7B model fine-tuned on the Bhagavad Gita Q&A dataset to provide spiritually grounded and therapeutic responses.


## 📂 Repository Structure

```bash
Gita-LLM/
├── data/                   # Datasets
├── notebooks/               # Fine-tuning scripts and configs
│   ├── data-processing.ipynb
│   └── dataset-creation.ipynb
│   └── Fine_tuning_GitaLLM_unsloth.ipynb (run on Google Colab)
│   └── QnA_dataset.ipynb
│   └── Running_Gita_LLM_(GPU).ipynb (run on Google Colab)
├── requirements.txt        # Python dependencies
└── README.md               # Project documentation
```

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/serpentile-c137/Gita-LLM.git
cd Gita-LLM
```

### 2. Install Dependencies

Make sure you have Python ≥3.11 and install dependencies:

```bash
pip install -r requirements.txt
```

### 3. Download the Dataset

The dataset is hosted on Hugging Face. Load it with:

```python
from datasets import load_dataset

dataset = load_dataset("serpentilec137/gita-verse-qna-dataset")
```
### 4. Fine-tune the Model

Use [Unsloth](https://github.com/unslothai/unsloth) for efficient fine-tuning:

```bash
notebooks/Fine_tuning_GitaLLM_unsloth.ipynb
```

Configuration can be customized in `training/config.yaml`.

### 5. Run model

Use the model and script from the below notebook (note: runnung model required GPU with CUDA cores):

```bash
notebooks/Running_Gita_LLM_(GPU).ipynb
```

You can integrate this with a web UI, CLI, or API service for interactive use.

---

## 🧘 Sample Use Case

**User:** *"I feel lost and anxious. What should I do?"*  
**Gita-LLM:** *"Perform your duty with devotion, without attachment to success or failure. Peace comes to those who act without selfish desires — Bhagavad Gita 2.47."*

---

## 🛠️ Technologies Used

- [Mistral 7B](https://mistral.ai/)
- [Unsloth](https://github.com/unslothai/unsloth)
- Python (3.10+)
- Hugging Face Transformers & Datasets
- PyTorch / CUDA

## 📚 Dataset Info

The dataset consists of question-answer pairs derived from interpretations of the Bhagavad Gita. It is intended for educational and therapeutic use.

Url: 
```bash
https://huggingface.co/datasets/serpentilec137/gita-verse-qna-dataset
```

## 🙏 Disclaimer

This project is **not a substitute for professional mental health care**. It is an experimental AI designed to share philosophical reflections inspired by the Bhagavad Gita.

## 📜 License

This project is open-sourced under the [Apache License](LICENSE).

## 🤝 Contributing

Contributions, ideas, and feedback are welcome! Feel free to:
- Fork the repo
- Open issues or pull requests
- Suggest improvements or expansions to the dataset

## 🌐 Connect

For collaboration or questions, feel free to reach out or open an issue.

---

🕊️ *"Let your mind be still, like a lamp in a windless place."* — *Bhagavad Gita*
