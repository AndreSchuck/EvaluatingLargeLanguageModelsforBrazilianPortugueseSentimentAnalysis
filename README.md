# Evaluating Large Language Models for Brazilian Portuguese Sentiment Analysis

This repository contains all resources, code, and data used in the research **"Evaluating Large Language Models for Brazilian Portuguese Sentiment Analysis: A Comparative Study of Multilingual State-of-the-Art vs. Brazilian Portuguese Fine-Tuned LLMs"**, submitted to the Journal of the Brazilian Computer Society (JBCS).

## 📖 About the Research

This study presents a comprehensive comparative analysis of 23 Large Language Models (LLMs) for sentiment analysis in Brazilian Portuguese texts, evaluating 13 state-of-the-art multilingual models and 10 Portuguese-specialized models through the in-context learning (ICL) paradigm.

### Key Contributions

- Comparative evaluation of large-scale LLMs (>70B parameters) vs. small-scale LLMs (<13B parameters)
- Analysis of the impact of linguistic specialization in Brazilian Portuguese
- Benchmarking across 12 public sentiment analysis datasets

## 🗂️ Repository Structure

## 📊 Evaluated Datasets

The study utilized 12 public Brazilian Portuguese sentiment analysis datasets:

### Translated Datasets

- **IMDB_PT**: Translated movie reviews
- **SST2_PT**: Translated Stanford Sentiment Treebank

### Native Datasets

- **TweetSentBr**: Social media posts
- **ReLI**: Book reviews
- **Computer-BR**: Computer-related posts
- **MTMSLA**: Social media posts
- **CSP-Eletrônicos**: Electronic product reviews
- **CSP-Livros**: Book reviews
- **4P Corpus**: Product reviews
- **RePro**: E-commerce reviews
- **OPCovidBR**: COVID-19 related posts
- **TA-Restaurantes**: Restaurant reviews

## 🤖 Evaluated Models

### Generalist Models (>70B parameters)

- Claude-3.5-Sonnet
- GPT-4o
- Gemini-1.5-Pro
- DeepSeek-V3

### PT-BR Specialized Models (>70B parameters)

- Sabiá-3
- Sabiá-2-Medium

### Generalist Models (<13B parameters)

- LLaMA-3/3.1-8B-Instruct
- Gemma-7B/2-9B-Instruct
- Qwen-2-7B-Instruct
- InternLM-2-7B-Chat
- DeepSeek-R1-Distill (7B/8B)

### PT-BR Specialized Models (<13B parameters)

- Bode Family (7B, 13B, 3.1-8B)
- Cabra Family (LLaMA-3-8B, Mistral-7B)
- Sabiá-7B
- GemBode and InternLM-ChatBode variants

## 📈 Main Results

- **Large-scale models** achieved accuracy exceeding 92%
- **Small-scale models** top performers reached accuracy above 90%
- **Linguistic specialization** showed mixed results, reducing hallucinations but not always improving performance
- **Newer models** consistently outperformed previous versions
- **All LLMs** significantly surpassed traditional machine learning methods

## 📋 Methodology

### In-Context Learning (ICL)

- **6 demonstrations** randomly selected per dataset
- **Structured prompt** in Brazilian

## 📈 Main Results

- **Large-scale models** achieved accuracy exceeding 92%
- **Small-scale models** top performers reached accuracy above 90%
- **Linguistic specialization** showed mixed results, reducing hallucinations but not always improving performance
- **Newer models** consistently outperformed previous versions
- **All LLMs** significantly surpassed traditional machine learning methods

## 📋 Methodology

### In-Context Learning (ICL)

- **6 demonstrations** randomly selected per dataset
- **Structured prompt** in Brazilian Portuguese with JSON specification
- **Binary classification** (positive/negative)

### Evaluation Metrics

- **Accuracy**: Primary metric
- **Macro F1 Score**: Complementary metric for imbalanced datasets
- **Hallucination rate**: Responses outside expected format

### Statistical Analysis

- **Wilcoxon test** for paired samples (α = 5%)
- **Comparative analysis** between model categories

## 📄 Citation

If you use this work, please cite:

```bibtex

```

## 🤝 Contributing

Contributions are welcome! For more information on how to contribute, see our [contribution guide](CONTRIBUTING.md).

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👥 Authors

- **André da Fonseca Schuck** - UNESP - [andre.schuck@unesp.br](mailto:andre.schuck@unesp.br)
- **Gabriel Lino Garcia** - UNESP - [gabriel.lino@unesp.br](mailto:gabriel.lino@unesp.br)
- **João Renato Ribeiro Manesco** - UNESP - [joao.r.manesco@unesp.br](mailto:joao.r.manesco@unesp.br)
- **Pedro Henrique Paiola** - UNESP - [pedro.paiola@unesp.br](mailto:pedro.paiola@unesp.br)
- **João Paulo Papa** - UNESP - [joao.papa@unesp.br](mailto:joao.papa@unesp.br)

## 🙏 Acknowledgments

We thank Maritaca AI for providing credits that made this study possible, FAPESP (grants 2013/07375-0, 2023/14427-8, and 2024/00789-8), and CNPq (grants 308529/2021-9 and 400756/2024-2) for financial support.

---

**Note**: This repository is constantly being updated. For the latest version of results and code, check the `main` branch.
