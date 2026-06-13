# 02 — Neural Bigrama

Primeira rede neural da trilha.

Neste notebook transformamos o modelo de bigramas construído anteriormente em uma rede neural simples utilizando PyTorch.

O objetivo não é criar um modelo melhor que o do Notebook 01, mas compreender como uma rede neural pode aprender as mesmas probabilidades através de parâmetros treináveis.

Aqui surgem pela primeira vez os conceitos fundamentais que aparecem em praticamente todos os modelos modernos de IA, desde pequenas redes neurais até os grandes modelos de linguagem atuais.

---

## O que você vai aprender

- O que são parâmetros treináveis
- Como representar conhecimento usando matrizes de pesos
- O que são logits
- Como transformar logits em probabilidades com Softmax
- O que é uma função de perda (Loss)
- Como funciona o treinamento de uma rede neural
- O que são gradientes
- Como funciona o Backpropagation
- O que é Gradient Descent
- O que é um Training Loop
- Como gerar texto utilizando uma rede neural

---

## O que mudou em relação ao Notebook 01?

No modelo clássico:

```text
Token Atual
↓
Tabela de Probabilidades
↓
Próximo Token
```

No modelo neural:

```text
Token Atual
↓
Matriz de Pesos
↓
Logits
↓
Softmax
↓
Probabilidades
↓
Próximo Token
```

A grande diferença é que agora as probabilidades não são calculadas diretamente a partir das contagens observadas.

Elas são aprendidas automaticamente durante o treinamento.

---

## Pré-requisitos

É recomendado ter concluído o notebook:

- 01 — Bigrama

Conhecimentos úteis:

- Tokenização
- Vocabulário
- Bigramas
- Probabilidade condicional

Não é necessário conhecimento prévio de redes neurais ou PyTorch.

---

## Dependências

```bash
pip install torch jupyter
```

---

## Como executar

```bash
cd notebooks/02_neural_bigrama
jupyter notebook notebook.ipynb
```

---

## Próximo passo

Neste notebook aprendemos a substituir uma tabela de contagens por parâmetros treináveis.

No próximo capítulo atacaremos uma limitação que continua existindo tanto no bigrama clássico quanto no neural:

```text
Apenas um token de contexto
```

Para isso estudaremos:

**03 — Markov**

onde começaremos a expandir o contexto utilizado pelo modelo.

```text
01 - Bigrama
↓
02 - Neural Bigrama ← você está aqui
↓
03 - Markov
↓
04 - HMM
↓
05 - Redes Neurais Profundas
↓
06 - Embeddings
↓
07 - Attention
↓
08 - Transformers
↓
09 - LLMs
```

---

## Conceito Central

Este notebook marca a transição entre estatística clássica e aprendizado por gradiente.

Pela primeira vez o conhecimento deixa de ser armazenado explicitamente em contagens e passa a ser representado por parâmetros aprendidos.

```text
Pesos
↓
Logits
↓
Softmax
↓
Loss
↓
Gradiente
↓
Backpropagation
↓
Gradient Descent
```

Compreender esses conceitos é muito mais importante do que memorizar código.

Eles serão reutilizados em todos os próximos notebooks da trilha.
