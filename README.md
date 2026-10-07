# Predictive Justice – Bias Analysis

**Cenário 5: Avaliação de Risco e Segurança Pública (COMPAS)**

Estudo de caso em Python: sub-representar intencionalmente um grupo étnico/racial no conjunto de
treinamento do COMPAS (ProPublica) e mostrar como isso gera taxas de erro díspares entre os grupos.

## Abrir no Colab

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ibgrilo/predictive-justice-bias-analysis/blob/main/notebooks/cenario5_compas.ipynb)

O notebook baixa o CSV direto do GitHub do ProPublica, então não precisa do submódulo. O link só funciona depois do push.

## Estrutura

```
data/compas-analysis/   submódulo git com os dados do ProPublica (propublica/compas-analysis)
docs/                   enunciado do seminário
notebooks/              cenario5_compas.ipynb (estudo de caso completo)
src/                    código reutilizável (filtros, treino, métricas)
```

## Como rodar

```bash
git clone --recurse-submodules https://github.com/ibgrilo/predictive-justice-bias-analysis.git
pip install -r requirements.txt
```

Se já clonou sem `--recurse-submodules`: `git submodule update --init`.

## Dados

Base: [ProPublica COMPAS](https://github.com/propublica/compas-analysis) (Broward County).
