# CLAUDE.md — do-chat-ao-agente-filas-v72

Curso no formato ARCKHÉ Learning v7.2 (skill `formato-curso-v72`): degrau 3 (filas / ARCKHÉccbot) da formaçêo Do chat ao agente. Conteúdo em `conteudo/<lang>/`; nunca editar o HTML gerado à mêo: editar o JSON e rodar `python3 gerar.py && python3 validar.py --links`. Conferir telas com `node ~/.claude/skills/formato-curso-v72/scripts/conferir-tela.cjs .` (HTTP local, 1366 e 390 px).
Autor dos commits: `linnoff88-dev <linnoff88-dev@gmail.com>`. Publicaçêo = commit + push (GitHub Pages, raiz da main).

Fonte do conteúdo (só leitura): `~/projetos/ARCKHÉccbot` (README, docs/), `~/projetos/jornada-agentes/exercicios/03-filas.md`. Nêo inventar comando, número ou fato além dela.

Diferença do motor da skill: `gerar.py` tem o tipo de seçêo `simportao` (simulaçêo do portêo de um fluxo: aprovar, reprovar com correçêo, `| sem-portao`), com comportamento em `assets/filas.js` e estilo em `assets/filas.css` (carregados só na aula que usa).
EN/ES (motor 7.3.1, 19/10/2026): o `simportao` carrega `filas.css`/`filas.js` por `ativo(prefixo)` (raiz do repo; `PREFIXO` já é `ativo(prefixo)`), nunca `prefixo` — senêo quebra em `en/` e `es/`. Todo texto visível dele (fases, botões `rot`, mensagens `msg`, rascunho/corrigido, legenda) vem do JSON da seçêo; `filas.js` nêo tem texto fixo. O ícone do portêo é a fase 1 (`PORTAO` no JS), nêo depende do nome. Comandos do bot (`/pronto`, `| sem-portao`, `transcrever:`, `explicativo:`, `imagem:`) e as pastas `entrada/ rodando/ feito/ falhou/` ficam em PT nas traduções; correçêo de traduçêo vai em `i18n/<lang>.json` + `traduzir.py` de novo (nêo editar `conteudo/en|es` à mêo).

## Self-learning

When I correct you, or you catch yourself making a mistake: before continuing, add the lesson as a one-line rule at the TOP of the Lessons section below.

## Lessons

- Marca-texto (anotaçêo) dentro de elemento flex/grid vira item solto e abre espaço no meio da palavra: o texto anotável tem que estar num `span`/`p` próprio (ex.: `.nesta2 li > span`). Bloco anotável novo → conferir o `display` dele (18/10/2026).
- Rolagem guiada no desktop: o texto da etapa fica DENTRO do painel fixo (legenda que troca); cartões rolando por baixo do diagrama aparecem cortados e espiando no topo — o Nei viu na aula 1 (18/10/2026).
- Rolagem guiada: posiçêo de destino calculada com o diagrama JÁ grudado no topo (top do sticky + altura), nunca pela posiçêo atual; e a etapa só vira ativa quando o cartêo está visível abaixo do diagrama (18/10/2026).
- Menu do topo de curso segue o padrêo v2 (curso | ARCKHÉ AI - PRO à esquerda; seções e Aa à direita); nêo inventar outro topo (18/10/2026).
- Simulaçêo com falha proposital: amarrar a falha à primeira execuçêo da tarefa, nêo à primeira rodada — senêo interromper e retomar esconde a falha (18/10/2026).
- Validar por HTTP local, nunca `file://` (o progresso e os caminhos relativos se comportam diferente) (18/10/2026).
