# 02 — Neural Bigrama

Segundo notebook da trilha. Aqui mantemos a mesma essência do modelo anterior (olhar um caractere para trás para prever o próximo), mas substituímos a tabela estática de contagens por uma **rede neural simples** de uma única camada linear.

Os parâmetros do modelo (os pesos da matriz) agora são aprendidos a partir de dados usando **gradiente descendente** e retropropagação (backpropagation), utilizando a biblioteca **PyTorch**.

---

## O que você vai aprender

- Como estruturar um dataset como pares de treinamento $(x, y)$ (token atual $\rightarrow$ próximo token)
- O que é e como funciona o **One-hot Encoding**
- Como a multiplicação de matrizes simula uma consulta de pesos para um caractere
- O que é a função **Softmax** e como ela transforma números quaisquer em probabilidades
- O conceito de **Cross-Entropy Loss** (função de perda de entropia cruzada)
- O fluxo de treinamento de uma rede neural:
  1. *Forward Pass* (calcula as previsões)
  2. *Loss Evaluation* (mede o erro)
  3. *Backward Pass* (calcula os gradientes automaticamente via PyTorch Autograd)
  4. *Parameter Update* (ajusta os pesos com gradiente descendente)

---

## Pré-requisitos

- Python básico (listas, dicionários, loops)
- **PyTorch** instalado (no ambiente virtual `.venv`)
- `matplotlib` para visualizações

---

## Como executar

```bash
cd notebooks/02_neural_bigrama
jupyter notebook notebook.ipynb
```

---

## Trilha completa

| # | Tema | Status |
|---|------|--------|
| 01 | Bigrama | ✅ |
| 02 | Neural Bigrama | ✅ |
| 03 | Markov | em breve |
| 04 | HMM | em breve |
| 05 | Redes Neurais | em breve |
| 06 | Embeddings | em breve |
| 07 | Attention | em breve |
| 08 | Transformers | em breve |
| 09 | LLMs | em breve |

→ Próximo: `03_markov`
