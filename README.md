# Predictive Justice – Bias Analysis

Seminário de Viés (P1) – **Cenário 5: Avaliação de Risco e Segurança Pública (COMPAS)**.

Estudo de caso em Python: sub-representar intencionalmente um grupo étnico/racial no conjunto de
treinamento do COMPAS (ProPublica) e mostrar como isso gera taxas de erro díspares entre os grupos.

## Estrutura

```
data/compas-analysis/   submódulo git com os dados do ProPublica (propublica/compas-analysis)
docs/                   enunciado do seminário
notebooks/              notebooks do estudo de caso
src/                    código reutilizável (filtros, treino, métricas)
```

## Como rodar

```bash
git clone --recurse-submodules <url-do-repo>
pip install -r requirements.txt
```

Se já clonou sem `--recurse-submodules`: `git submodule update --init`.

## Roteiro da apresentação

1. Explicar o código + discussão ética/técnica.
2. Mostrar a etapa exata em que o desequilíbrio populacional artificial é criado.
3. Explicar o mecanismo do viés (onde o modelo falha nos positivos do grupo minoritário).
4. Propor mitigação.

## Dados

Base: [ProPublica COMPAS](https://github.com/propublica/compas-analysis) (Broward County).
