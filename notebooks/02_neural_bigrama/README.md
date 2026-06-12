# 02 — Neural Bigram

Primeiro contato com Deep Learning na trilha.

Neste notebook transformamos o modelo de bigramas construído anteriormente em uma rede neural simples utilizando PyTorch.

O objetivo não é criar um modelo melhor que o do Notebook 01, mas compreender como uma rede neural pode aprender as mesmas probabilidades através de parâmetros treináveis, introduzindo os conceitos fundamentais que aparecem em praticamente todos os modelos modernos de IA.

---

## O que você vai aprender

- O que são parâmetros treináveis
- Como representar conhecimento usando matrizes de pesos
- O que são logits
- Como transformar logits em probabilidades com Softmax
- O que é uma função de perda (Loss)
- Como funciona o treinamento de uma rede neural
- O que são gradientes e Backpropagation
- Como uma rede aprende a prever o próximo token

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

Elas serão aprendidas automaticamente durante o treinamento.

---

## Pré-requisitos

É recomendado ter concluído o notebook:

- 01 — Bigrama

Conhecimentos úteis:

- Conceito de tokenização
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
cd notebooks/02_neural_bigram
jupyter notebook notebook.ipynb
```

---

## Próximo passo

Após concluir este notebook você estará preparado para estudar representações distribuídas e embeddings, onde os tokens deixam de ser apenas identificadores e passam a adquirir significado vetorial.

```text
01 - Bigrama
↓
02 - Neural Bigram ← você está aqui
↓
03 - Embeddings
↓
04 - MLP
↓
05 - Attention
↓
06 - Mini GPT
```

---

## Conceito Central

Este notebook marca a transição entre estatística clássica e Deep Learning.

Aqui surgem pela primeira vez os conceitos que aparecem em praticamente todas as arquiteturas modernas de IA:

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
```

Compreender esses conceitos é muito mais importante do que memorizar código.

Eles serão reutilizados em todos os próximos notebooks da trilha.