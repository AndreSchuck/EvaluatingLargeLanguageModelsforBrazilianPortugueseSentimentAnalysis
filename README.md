# Evaluating Large Language Models for Brazilian Portuguese Sentiment Analysis

This repository contains all resources, code, and data used in the research **"Evaluating Large Language Models for Brazilian Portuguese Sentiment Analysis: A Comparative Study of Multilingual State-of-the-Art vs. Brazilian Portuguese Fine-Tuned LLMs"**, submitted to the Journal of the Brazilian Computer Society (JBCS).

## 📖 About the Research

This study presents a comprehensive comparative analysis of 23 Large Language Models (LLMs) for sentiment analysis in Brazilian Portuguese texts, evaluating 13 state-of-the-art multilingual models and 10 Portuguese-specialized models through the in-context learning (ICL) paradigm.

### Key Contributions

- Comparative evaluation of large-scale LLMs (>70B parameters) vs. small-scale LLMs (<13B parameters)
- Analysis of the impact of linguistic specialization in Brazilian Portuguese
- Benchmarking across 12 public sentiment analysis datasets

## 🗂️ Repository Structure

```bash
.
│   README.md
│
├───datasets
│   ├───preprocessed
│   │   │   readme.md
│   │   │
│   │   ├───Computer-BR
│   │   │       computer-br_demo.csv
│   │   │       computer-br_test.csv
│   │   │       computer-br_train.csv
│   │   │
│   │   ├───Corpus-4p
│   │   │       corpus-4p_demo.csv
│   │   │       corpus-4p_test.csv
│   │   │       corpus-4p_train.csv
│   │   │
│   │   ├───CSP_Eletronicos
│   │   │       csp-eletronicos_demo.csv
│   │   │       csp-eletronicos_test.csv
│   │   │       csp-eletronicos_train.csv
│   │   │
│   │   ├───CSP_Livros
│   │   │       csp-livros_demo.csv
│   │   │       csp-livros_test.csv
│   │   │       csp-livros_train.csv
│   │   │
│   │   ├───IMDB_PT
│   │   │       imdb-pt_demo.csv
│   │   │       imdb-pt_test.csv
│   │   │       imdb-pt_train.csv
│   │   │
│   │   ├───MTMSLA
│   │   │       mtmsla_demo.csv
│   │   │       mtmsla_test.csv
│   │   │       mtmsla_train.csv
│   │   │
│   │   ├───OPCovidBR
│   │   │       opcovidbr_demo.csv
│   │   │       opcovidbr_test.csv
│   │   │       opcovidbr_train.csv
│   │   │
│   │   ├───ReLI
│   │   │       reli_demo.csv
│   │   │       reli_test.csv
│   │   │       reli_train.csv
│   │   │
│   │   ├───RePRO
│   │   │       repro_demo.csv
│   │   │       repro_test.csv
│   │   │       repro_train.csv
│   │   │
│   │   ├───SST2_PT
│   │   │       sst2-pt_demo.csv
│   │   │       sst2-pt_test.csv
│   │   │       sst2-pt_train.csv
│   │   │
│   │   ├───TA-Restaurantes
│   │   │       ta-restaurantes_demo.csv
│   │   │       ta-restaurantes_test.csv
│   │   │       ta-restaurantes_train.csv
│   │   │
│   │   └───TweetSentBR
│   │           tweet-sent-br_demo.csv
│   │           tweet-sent-br_test.csv
│   │           tweet-sent-br_train.csv
│   │
│   └───raw
│       │   readme.md
│       │
│       ├───Computer-BR
│       │       Computer-BR.xlsx
│       │       readme.md
│       │
│       ├───Corpus-4p
│       │       10.txt
│       │       11.txt
│       │       30.txt
│       │       31.txt
│       │       readme.md
│       │
│       ├───CSP_Eletronicos
│       │       readme.md
│       │       sentencas.xlsx
│       │
│       ├───CSP_Livros
│       │       corpus_book_reviews_portuguese.csv
│       │       readme.md
│       │
│       ├───IMDB_PT
│       │       readme.md
│       │       test-all.csv
│       │       train.csv
│       │
│       ├───MTMSLA
│       │       mtmsla.xlsx
│       │       readme.md
│       │
│       ├───OPCovidBR
│       │       opcovidbr.csv
│       │       readme.md
│       │
│       ├───ReLI
│       │       readme.md
│       │       ReLi-Amado.txt
│       │       ReLi-Meyer.txt
│       │       ReLi-Orwell.txt
│       │       ReLi-Reboucas.txt
│       │       ReLi-Salinger.txt
│       │       ReLi-Saramago.txt
│       │       ReLi-Sheldon.txt
│       │
│       ├───RePRO
│       │       readme.md
│       │       RePro.csv
│       │
│       ├───SST2_PT
│       │       readme.md
│       │       train.csv
│       │       validation.csv
│       │
│       ├───TA-Restaurantes
│       │       POL_restaurants.tsv
│       │       readme.md
│       │
│       └───TweetSentBR
│               readme.md
│               test-00000-of-00001.parquet
│               train-00000-of-00001.parquet
│
└───notebooks
    ├───datasets
    │       datasets_preprocessing.ipynb
    │
    └───models
            bode_13b.ipynb
            bode_3_1_8b_instruct_lora.ipynb
            bode_7b.ipynb
            cabrallama_3_8b.ipynb
            cabramistral_v3_7b_32k.ipynb
            claude_3_5_sonnet.ipynb
            deepseek_r1.ipynb
            deepseek_r1_distill_llama_8b.ipynb
            deepseek_r1_distill_qwen_7b.ipynb
            deepseek_v3.ipynb
            gembode_7b_instruct.ipynb
            gemini_1_5_pro.ipynb
            gemma_2_9b_instruct.ipynb
            gemma_7b_instruct.ipynb
            gpt_4o.ipynb
            Internlm_2_7b_chat.ipynb
            InternLM_chatbode_7b.ipynb
            llama_3_1_8b_instruct.ipynb
            llama_3_8b_instruct.ipynb
            qwen_2_7b_instruct.ipynb
            sabia_2_medium.ipynb
            sabia_3.ipynb
            sabia_7b.ipynb
```

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
- DeepSeek-R1

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
@article{Schuck_Garcia_Manesco_Paiola_Papa_2025,
	title        = {Evaluating Large Language Models for Brazilian Portuguese Sentiment Analysis: A Comparative Study of Multilingual State-of-the-Art vs. Brazilian Portuguese Fine-Tuned LLMs},
	author       = {Schuck, André da Fonseca and Garcia, Gabriel Lino and Manesco, João Renato Ribeiro and Paiola, Pedro Henrique and Papa, João Paulo},
	year         = {2025},
	month        = {Oct.},
	journal      = {Journal of the Brazilian Computer Society},
	volume       = {31},
	number       = {1},
	pages        = {885–917},
	doi          = {10.5753/jbcs.2025.5793},
	url          = {https://journals-sol.sbc.org.br/index.php/jbcs/article/view/5793}
}
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
