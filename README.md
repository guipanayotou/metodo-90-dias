# Método 90 Dias

Programa guiado de 90 dias para fazer a IA (ChatGPT, Google AI Mode, Perplexity) indicar o seu negócio.

**Site:** https://guipanayotou.github.io/metodo-90-dias/

| Peça | O que faz |
|---|---|
| **Calendário** | 18 tarefas distribuídas nas datas reais a partir da sua data de início. Toque num dia e veja exatamente o que fazer nele. |
| **Medição** | Registro diário por motor, com taxa de detecção e intervalo de confiança de 95% (Wilson, com correção de agrupamento). |
| **Diagnóstico** | Assistente que separa os três problemas possíveis — qualidade, página e recuperação — e cria a tarefa de reparo no calendário. |
| **Fichas** | Oito referências curtas com a evidência que sustenta cada tarefa. |

## Como funciona por dentro

Arquivo único, sem build. React 18 + htm e Day.js, carregados de CDN. Os gráficos são SVG escritos à mão.
Instalável como app no celular (manifest) e funciona sem internet (service worker, rede-primeiro).

Os dados ficam no `localStorage` do navegador — nada sai do aparelho. Para levar o programa para outro
aparelho, use **Ajustes → Baixar backup** e carregue o arquivo no destino.

### Sincronizar entre aparelhos

O adaptador de Supabase está escrito e comentado no topo do módulo de dados, dentro do `index.html`:
traz o SQL das tabelas, as duas funções `security definer` e os `grant`/`revoke`. Para ligar, preencha
`SUPABASE_URL` e `SUPABASE_CHAVE` e troque `let SINC = null` por `let SINC = sincSupabase()`.

**Modelo de segurança, sem enfeite:** quem souber o código do espaço lê e escreve aquele registro — é o
nível de um link não listado. Para uso multicliente de verdade, troque as funções por RLS sobre
`auth.uid()` com login por e-mail.

## Limites, declarados

Os percentuais citados nas fichas vêm de estudos majoritariamente em inglês e com dados dos Estados
Unidos. Não existe, até setembro de 2026, benchmark público sólido sobre quais fontes a IA cita em
perguntas em português. Trate-os como direção, não como valores do seu setor — o seu número só sai
medindo o seu caso.

Nenhuma técnica aqui tem efeito causal comprovado sobre receita. O que está sustentado é influência
sobre citação, e mesmo essa varia por motor e ao longo do tempo.
