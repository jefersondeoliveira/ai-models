# 01 — Bigrama

Primeiro notebook da trilha.

Aqui construiremos do zero um modelo de linguagem baseado em bigramas utilizando apenas Python puro e um dataset extremamente pequeno.

O objetivo não é criar um modelo poderoso, mas compreender os princípios fundamentais que estão na base de praticamente todos os modelos de linguagem modernos, incluindo os LLMs.

Ao final deste notebook você terá construído seu primeiro modelo capaz de aprender padrões estatísticos e gerar texto.

---

## O que você vai aprender

- O que é um token
- O que é um vocabulário
- Como converter texto em números (tokenização)
- O que são bigramas
- O que é uma probabilidade condicional
- Como um modelo prevê o próximo token
- Como gerar texto de forma autoregressiva
- Por que contexto limitado é um problema fundamental

---

## O que vamos construir?

Nosso modelo seguirá um fluxo simples:

```text
Texto
↓
Vocabulário
↓
Tokenização
↓
Bigramas
↓
Probabilidades
↓
Geração de Texto
```

Embora extremamente simples, essa estrutura já contém várias ideias fundamentais presentes em sistemas modernos de IA.

---

## O que é um Bigrama?

Um bigrama é simplesmente um par de tokens consecutivos.

Exemplo:

```text
Texto:

ola

Tokens:

o → l → a

Bigramas:

(o, l)
(l, a)
```

A partir desses pares, o modelo aprende quais tokens costumam aparecer após outros tokens.

---

## Limitações do Modelo

Nosso modelo consegue observar apenas um token anterior.

Em outras palavras:

```text
Token Atual
↓
Próximo Token
```

Todo o restante do contexto é descartado.

Essa limitação será a principal motivação para os próximos notebooks da trilha.

---

## Pré-requisitos

Conhecimentos úteis:

- Python básico
- Listas
- Dicionários
- Loops

Nenhum conhecimento prévio sobre Machine Learning ou Inteligência Artificial é necessário.

---

## Dependências

Este notebook utiliza apenas bibliotecas da própria linguagem Python.

Nenhuma dependência externa é necessária.

---

## Como executar

```bash
cd notebooks/01_bigrama
jupyter notebook notebook.ipynb
```

---

## Próximo passo

Após concluir este notebook você estará preparado para estudar como uma rede neural pode aprender exatamente as mesmas probabilidades sem utilizar tabelas explícitas de contagem.

```text
01 - Bigrama ← você está aqui
↓
02 - Neural Bigram
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

Todo modelo de linguagem tenta responder uma única pergunta:

```text
Dado o contexto atual,
qual token deve vir em seguida?
```

Neste notebook responderemos essa pergunta utilizando apenas contagens e probabilidades.

Nos próximos notebooks veremos abordagens cada vez mais sofisticadas para resolver exatamente o mesmo problema.