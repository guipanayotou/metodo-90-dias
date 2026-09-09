# Método 90 Dias

Programa guiado de 90 dias — o app do método **AIndicação · 12 semanas** — para fazer a IA (ChatGPT,
Modo IA do Google, Perplexity) indicar o seu negócio e provar, com faixa de erro, se alguma coisa mudou.

**Site:** https://guipanayotou.github.io/metodo-90-dias/

## O que é

Um app de página única, sem back-end. Tudo fica no seu navegador — nada é enviado a servidor nenhum.

| Aba | O que faz |
|---|---|
| **Hoje** | A sequência do dia: entender → verificar → fazer → medir. |
| **Programa** | As 5 fases, as 18 tarefas do Anexo A e os 4 marcos, em lista e em calendário. |
| **Ferramentas** | Medição com rotação diária e faixa de erro, diagnóstico guiado, carteira de perguntas, as 12 verificações técnicas pelo jeito simples (navegador e ferramentas gratuitas, sem terminal), o checklist do Perfil da Empresa no Google (Local) e o banco de 30 prompts do livro — mais a FICHA do assistente montada com os seus dados (Assistente). |
| **Livro** | A teoria inteira em 67 seções, ligada a cada tarefa e a cada conceito. |

## O livro

O sistema é a execução do livro **“Faça as IAs te indicarem”** — método AIndicação · 12 semanas (173 páginas, 17 capítulos e 9 anexos).
O livro ensina e traz as fontes; o app executa. Cada capítulo do livro tem, aqui dentro, a tela
que faz o trabalho — e cada seção do app diz de qual capítulo ela veio.

## Método, em uma linha

De 20 a 30 perguntas fechadas, 3 motores, 7 rodadas por pergunta, 5 perguntas por dia em rotação,
24 dias antes de qualquer conclusão e nenhuma leitura decisória antes do dia 76. Todo número sai com
faixa de erro e número de rodadas.

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
