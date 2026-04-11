# Revisão Sistemática — Manuscrito (espelho público)

Este repositório contém o manuscrito LaTeX (PT-BR, ABNT) da revisão sistemática da
literatura conduzida como Etapa 1 da dissertação de mestrado no Programa de
Pós-Graduação em Computação Aplicada (PPGPCA) da Universidade Federal da Fronteira
Sul (UFFS).

O repositório é um **espelho publicado para leitura e revisão**. A fonte canônica
do manuscrito reside em um workspace privado e é sincronizada automaticamente para
este espelho após cada passagem pelo gate de controle de qualidade do pipeline de
escrita.

## Pacote de replicação

O pacote de replicação da revisão sistemática — protocolo PRISMA 2020, estratégia
de busca, decisões de triagem, dados de extração e síntese — está publicado em
repositório separado com DOI permanente via Zenodo:

- **Código e dados:** <https://github.com/alexandre-zatti/slr-code-agent-memory>
- **DOI permanente:** ver badge do Zenodo no repositório acima

## Estrutura

```
main.tex            documento principal
secoes/             seções individuais (método, resultados, discussão, ...)
figuras/            figuras TikZ
referencias/        bibliografia (estudos-incluidos.bib)
```

## Compilação

```bash
latexmk -pdf main.tex
```

Dependências: distribuição TeX Live recente com `abntex2`, `booktabs`, `tikz`.

## Licença

CC BY 4.0. Ao usar ou citar o conteúdo deste manuscrito, por favor referencie a
versão publicada em venue acadêmico (quando disponível) ou o DOI do pacote de
replicação em Zenodo.
