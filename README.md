# Revisão Sistemática — Persistência de Conhecimento em Agentes de Codificação

Revisão sistemática da literatura sobre arquiteturas de persistência de conhecimento em
agentes de codificação: como sistemas recentes armazenam, recuperam e reutilizam
experiência ao longo de tarefas de engenharia de software, e que evidências empíricas
existem sobre a eficácia e o custo dessas abordagens.

## Motivação

Agentes de codificação têm sido avaliados majoritariamente em configurações sem memória
entre tarefas. Isso oculta um conjunto de decisões de projeto — o que armazenar, como
recuperar, quando esquecer, quanto custa — que influenciam diretamente desempenho,
reprodutibilidade e custo de operação. Esta revisão mapeia o campo, organiza as
arquiteturas propostas em uma taxonomia comparável e confronta cada uma com as
evidências empíricas disponíveis.

## Questão de pesquisa

De que forma a literatura existente aborda a persistência de conhecimento em agentes de
codificação, e que evidências existem sobre a eficácia e o custo-eficiência de diferentes
arquiteturas de persistência?

## Método

Protocolo PRISMA 2020 com checklist PRISMA-S para a fase de busca. Buscas booleanas
reproduzíveis em Scopus e arXiv complementadas por citation chasing via Semantic Scholar.
Dos 1.194 registros identificados, 28 estudos primários foram incluídos após triagem em
duas fases e aplicação de critérios pré-registrados de inclusão e exclusão.

## Compilação

```
latexmk -pdf main.tex
```

Dependências: TeX Live recente com `abntex2`, `booktabs` e `tikz`.

## Contexto

Pesquisa conduzida no Programa de Pós-Graduação em Computação Aplicada (PPGPCA) da
Universidade Federal da Fronteira Sul (UFFS).

## Licença

CC BY 4.0.
