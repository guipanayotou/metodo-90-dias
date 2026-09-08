# Método 90 Dias

Programa guiado de 90 dias para fazer a IA (ChatGPT, Google AI Mode, Perplexity) indicar o seu
negócio — e para provar, com faixa de erro, se alguma coisa mudou.

**Site:** https://guipanayotou.github.io/metodo-90-dias/

## O que é

Um app de página única, sem back-end. Tudo fica no seu navegador — nada é enviado a servidor nenhum.

| Aba | O que faz |
|---|---|
| **Hoje** | A sequência do dia: entender → verificar → fazer → medir. |
| **Programa** | As 5 fases, 18 tarefas e 4 marcos, em lista e em calendário. |
| **Ferramentas** | Medição com faixa de confiança, diagnóstico guiado e carteira de perguntas. |
| **Livro** | A teoria inteira em 56 seções, ligada a cada tarefa e a cada conceito. |

## O livro

O sistema é a execução do livro **“Fazer a IA indicar você — Método 90 Dias”** (58 páginas).
O livro ensina e traz as fontes; o app executa. Cada capítulo do livro tem, aqui dentro, a tela
que faz o trabalho — e cada seção do app diz de qual capítulo ela veio.

## Método, em uma linha

De 20 a 30 perguntas congeladas, 3 motores, 7 repetições por pergunta por dia, janela de 24 dias
antes de qualquer leitura decisória. Todo número sai com faixa de erro e tamanho de amostra.

## Rodar localmente

```bash
python3 -m http.server 8080     # e abra http://localhost:8080
# ou
docker build -t metodo90 . && docker run -p 8080:80 metodo90
```

## Estrutura

- `index.html` — o app inteiro (HTML + CSS + JS, sem build)
- `manifest.json`, `sw.js`, `icone.svg` — instalável como PWA, funciona offline
- `Dockerfile` — servir estático em nginx

## Licença

© 2026 Guilherme Panayotou. Conteúdo e método reservados.
Os dados de terceiros citados pertencem às fontes indicadas em cada gráfico.
