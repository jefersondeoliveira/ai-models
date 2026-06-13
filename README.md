# AI Models — Do Bigrama aos LLMs

Uma trilha prática de estudos para compreender como modelos de linguagem funcionam internamente.

Ao invés de começar por frameworks complexos ou arquiteturas prontas, esta trilha reconstrói a evolução histórica dos modelos de IA passo a passo, partindo dos conceitos mais simples até chegar aos Large Language Models modernos.

O foco não é performance.

O foco é entendimento.

Ao final da jornada, você terá implementado os principais blocos conceituais que deram origem aos modelos atuais.

---

## Filosofia da Trilha

Cada notebook segue três princípios:

### 1. Construir antes de abstrair

Antes de utilizar componentes prontos, implementamos versões simples para entender como funcionam internamente.

### 2. Evolução histórica

Cada novo notebook surge para resolver uma limitação do anterior.

Isso permite entender não apenas *como* uma técnica funciona, mas também *por que ela foi criada*.

### 3. Aprendizado progressivo

Os conceitos são introduzidos gradualmente.

Cada etapa reutiliza conhecimentos adquiridos anteriormente.

---

## O que vamos construir?

Ao longo da trilha veremos a evolução dos modelos de linguagem:

```text
Texto
↓
Bigramas
↓
Modelos Probabilísticos
↓
Redes Neurais
↓
Embeddings
↓
Attention
↓
Transformers
↓
LLMs
```

A ideia central permanece a mesma durante toda a jornada:

```text
Dado o contexto atual,
qual token deve vir em seguida?
```

O que muda é a forma como cada modelo tenta responder essa pergunta.

---

## Trilha de Estudos

| # | Tema |
|---|------|
| [01 — Bigrama](notebooks/01_bigrama/) | Entender tokenização, probabilidades e geração de texto |
| [02 — Neural Bigram](notebooks/02_neural_bigrama/) | Introduzir pesos, logits, loss e treinamento |
| 03 — Markov | Expandir o contexto além de um único token |
| 04 — HMM | Introduzir estados ocultos e inferência probabilística |
| 05 — Redes Neurais | Compreender perceptrons, backpropagation e aprendizado |
| 06 — Embeddings | Transformar tokens em representações vetoriais densas |
| 07 — Attention | Aprender contexto dinâmico e relevância entre tokens |
| 08 — Transformers | Construir a arquitetura que revolucionou os LLMs |
| 09 — LLMs | Pré-treinamento, fine-tuning, RLHF e scaling laws |

---

## Progresso Atual

```text
✅ 01 — Bigrama
✅ 02 — Neural Bigram

🚧 03 — Markov
🚧 04 — HMM
🚧 05 — Redes Neurais
🚧 06 — Embeddings
🚧 07 — Attention
🚧 08 — Transformers
🚧 09 — LLMs
```

---

## Como Utilizar

Cada notebook é autocontido e possui seu próprio README com explicações detalhadas.

Recomenda-se seguir a ordem proposta pela trilha.

```bash
cd notebooks/01_bigrama
jupyter notebook notebook.ipynb
```

---

## Pré-requisitos

### Obrigatórios

- Python 3.10+
- Jupyter Notebook ou JupyterLab

### Bibliotecas

Os primeiros notebooks utilizam apenas Python puro.

À medida que avançamos na trilha, introduziremos bibliotecas como:

- NumPy
- PyTorch

Sempre explicando o que acontece por trás das abstrações.

---

## Estrutura do Projeto

```text
ai-models/
│
├── notebooks/
│   ├── 01_bigrama/
│   ├── 02_neural_bigram/
│   ├── 03_markov/
│   ├── 04_hmm/
│   ├── 05_redes_neurais/
│   ├── 06_embeddings/
│   ├── 07_attention/
│   ├── 08_transformers/
│   └── 09_llms/
│
└── data/
```

---

## Objetivo Final

Ao concluir esta trilha, você deverá ser capaz de explicar:

- Como texto vira números
- Como modelos aprendem padrões
- Como redes neurais são treinadas
- Como embeddings representam significado
- Como attention captura contexto
- Como transformers funcionam
- Como os LLMs modernos são construídos

Mais importante do que utilizar uma API será compreender os mecanismos que tornam esses modelos possíveis.
