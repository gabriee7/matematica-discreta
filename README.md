# COM06851 — Material de Estudo (Matemática Discreta)

Site estático (HTML/CSS puro + MathJax via CDN, sem build step) cobrindo **Probabilidade Discreta** e
**Comportamento Assintótico de Funções (O, Ω, Θ)**, com a resolução completa das 22 questões da Lista de
Exercícios III da disciplina COM06851 (UFES, Prof. Edmar Hell Kampke).

## Estrutura

```
/index.html                       landing page com sumário dos 6 módulos
/styles.css                       estilos compartilhados
/modulos/01-espaco-amostral.html
/modulos/02-espacos-equiprovaveis.html
/modulos/03-teoremas-adicao.html
/modulos/04-probabilidade-condicional.html
/modulos/05-independencia-tentativas.html
/modulos/06-comportamento-assintotico.html
/lista/lista-completa.html        as 22 questões, com link de volta para cada módulo
/fontes/                          PDFs originais das aulas e da lista (fonte primária do conteúdo)
```

## Publicação — GitHub Pages

O repositório remoto é: `https://github.com/gabriee7/matematica-discreta.git`

A branch usada para publicação é `main`, pasta raiz (`/`) — não há pasta `/docs` nem pipeline de build.

Como o ambiente local não tem a CLI `gh` autenticada, a ativação do GitHub Pages precisa ser feita
manualmente, pelos seguintes passos:

1. Acesse `https://github.com/gabriee7/matematica-discreta/settings/pages`.
2. Em **Build and deployment → Source**, selecione **Deploy from a branch**.
3. Em **Branch**, selecione `main` e a pasta `/ (root)`.
4. Clique em **Save**.
5. Após alguns minutos, o site ficará disponível em
   `https://gabriee7.github.io/matematica-discreta/`.

## Nota sobre o gabarito da Questão 18(b)

O PDF oficial da Lista III lista a resposta de 18(b) como `1-(0,6)⁵=0,07776`. Matematicamente,
\((0.6)^5 = 0.07776\), mas \(1-(0.6)^5 = 0.92224\) — o valor no gabarito parece ser um erro de transcrição
(foi anotado o valor de \((0.6)^5\) em vez de \(1-(0.6)^5\)). O site apresenta a fórmula corretamente
aplicada (resultado 0.92224) com uma nota explícita apontando essa divergência — ver
`modulos/05-independencia-tentativas.html#ex18`.

## Fontes

Todo o conteúdo teórico e os exercícios foram extraídos diretamente dos PDFs em `fontes/`:
- `COM06851-Aula 11.pdf` — Probabilidade Discreta.
- `COM06851-Aula 12.pdf` — Comportamento Assintótico de Funções.
- `COM06851-Lista III.pdf` — Lista de Exercícios (com gabarito das questões 1–19).

Um complemento pontual (fórmula de combinação \(C(n,k)\) e a distribuição binomial) foi adicionado por não
estar explícito nas aulas, mas ser necessário para resolver os exercícios — está sinalizado nas páginas com
a caixa "Complemento" tracejada.
