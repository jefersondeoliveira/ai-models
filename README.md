# AI Models — Do Bigrama aos LLMs

Uma trilha de estudos que constrói modelos de linguagem do zero, partindo dos conceitos mais simples até os transformers modernos.

Cada notebook é autocontido, progressivo e focado em compreensão — não em performance.

---

## Trilha

| # | Tema | Conceitos-chave |
|---|------|-----------------|
| [01 — Bigrama](notebooks/01_bigrama/) | Tokenização, vocabulário, probabilidade condicional, geração autoregressiva | ✅ |
| [02 — Neural Bigrama](notebooks/02_neural_bigrama/) | Rede neural simples, gradiente, substituindo contagens por pesos | ✅ |
| 03 — Markov | Contexto expandido, ordem N, cadeias de Markov | em breve |
| 04 — HMM | Estados ocultos, algoritmo de Viterbi | em breve |
| 05 — Redes Neurais | Perceptron, backpropagation, funções de ativação | em breve |
| 06 — Embeddings | Representação densa, word2vec, espaço vetorial | em breve |
| 07 — Attention | Mecanismo de atenção, contexto dinâmico | em breve |
| 08 — Transformers | Arquitetura completa, self-attention, positional encoding | em breve |
| 09 — LLMs | Pré-treino, fine-tuning, RLHF, scaling laws | em breve |

---

## Como usar

Cada pasta contém um `notebook.ipynb` e um `README.md` com instruções específicas.

```bash
cd notebooks/01_bigrama
jupyter notebook notebook.ipynb
```

## Pré-requisitos gerais

- Python 3.10+
- Jupyter Notebook ou JupyterLab
- Os notebooks iniciais não exigem bibliotecas externas
- Os notebooks avançados usarão numpy, pytorch e similares
