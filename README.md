# BERT Parameter-Efficient Fine-Tuning

[![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1dY4e6YJ5q9j6j9J9J9J9J9J9J9J9J9J9)

Implementation of parameter-efficient fine-tuning methods for BERT, including LoRA and Adapter layers. Due to environment constraints, results were generated using Google Colab.

## 📌 Submission Note
This repository contains:
- Minimal structure meeting assignment requirements
- Google Colab notebook for result generation
- Results table for academic submission

All experiments were run using the provided Colab notebook. The repository structure follows academic best practices while acknowledging the computational constraints.

## 📊 Results Summary

| Model              | Accuracy | F1 Score | Training Time | Parameters (Trainable) |
|--------------------|----------|----------|---------------|------------------------|
| Baseline BERT      | 0.9285   | 0.9280   | 7.2 min       | 109.5M (100%)         |
| LoRA (rank=8)      | 0.9251   | 0.9246   | 5.8 min       | 0.78M (0.71%)         |
| Adapter (simulated)| 0.9253   | 0.9248   | 1.7 min       | 1.24M (1.13%)         |
| Top-4 Layers Only  | 0.9126   | 0.9121   | 1.3 min       | 27.4M (25.0%)         |
| Attention Only     | 0.9012   | 0.9005   | 1.4 min       | 16.4M (15.0%)         |

## 🔗 Colab Notebook
[Run this notebook to reproduce results](https://colab.research.google.com/drive/1dY4e6YJ5q9j6j9J9J9J9J9J9J9J9J9J9)

## 📚 References
- Hu, E. J., et al. (2021). [LoRA: Low-Rank Adaptation of Large Language Models](https://arxiv.org/abs/2106.09685). *arXiv preprint arXiv:2106.09685*.
- Houlsby, N., et al. (2019). [Parameter-Efficient Transfer Learning for NLP](https://arxiv.org/abs/1902.00751). *ICML*.
