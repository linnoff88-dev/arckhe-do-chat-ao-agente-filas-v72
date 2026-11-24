# Filas: dez tarefas e vÃ¡ dormir â€” curso (ARCKHÉ Learning v7.2)

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="48" />
  <p><strong>Arckhé AI</strong></p>
</div>


Curso completo do **degrau 3** da formaÃ§Ã£o [Do chat ao agente](https://linnoff88-dev.github.io/ mandar vÃ¡rias tarefas para uma fila durÃ¡vel, sair de perto e encontrar o trabalho feito, com portÃ£o onde precisa de vocÃª. A ferramenta Ã© o [ARCKHÉccbot](https://linnoff88-dev.github.io/ (gateway do Telegram + fila durÃ¡vel).

**Abrir o curso:** https://linnoff88-dev.github.io/

**Other languages:** [English](https://linnoff88-dev.github.io/ Â· [EspaÃ±ol](https://linnoff88-dev.github.io/

## As 7 aulas

1. **Do chat Ã  fila** â€” as quatro garantias de uma fila durÃ¡vel.
2. **O que vai para a fila** â€” triagem em sozinha, com portÃ£o ou fica com vocÃª.
3. **A fila caseira em 30 linhas** â€” `fila-caseira.sh`, interromper e retomar (simulaÃ§Ã£o).
4. **Instalar o ARCKHÉccbot** â€” atÃ© o `/ping` responder; pareamento e segredos.
5. **Mandar o lote** â€” skills, as cinco filas, `/fila`, `/jobs`, cÃ³digo 143.
6. **PortÃµes** â€” fluxo com portÃ£o, `/pronto`, reprovar com correÃ§Ã£o, `| sombra` (simulaÃ§Ã£o).
7. **O dia seguinte** â€” conferir, medir as certas na primeira, regra nova e plano com datas.

## Como funciona

| Arquivo | O que Ã© |
|---|---|
| `conteudo/pt/curso.json` | nome, vÃ­deos, pÃ¡gina inicial e textos da interface |
| `conteudo/pt/aulas/*.json` | uma aula por arquivo |
| `gerar.py` | monta `index.html` e `aulas/<slug>/index.html` |
| `validar.py` | portÃ£o de qualidade (`--links` confere os links externos) |
| `assets/` | CSS, JS, imagens e legendas (`filas.js`/`filas.css`: simulaÃ§Ã£o do portÃ£o) |

```bash
python3 gerar.py && python3 validar.py --links
```

EN e ES (`en/`, `es/`): textos em `conteudo/en|es/`, gerados por `traduzir.py` da skill (Codex da assinatura, cache em `i18n/`); capa com texto em `assets/img/capa-en.jpg` e `capa-es.jpg`.

```bash
python3 ~/.claude/skills/formato-curso-v72/scripts/traduzir.py . en es
python3 gerar.py --lang en && python3 gerar.py --lang es
python3 validar.py --lang en && python3 validar.py --lang es
```

HTML estÃ¡tico, sem build e sem backend. O progresso fica sÃ³ no navegador de quem estuda.

VÃ­deos da sÃ©rie *Do chat ao agente* ([jornada-agentes](https://github.com/linnoff88-dev/jornada-agentes), release `video-v2.0.0`). ExercÃ­cios originais em [`exercicios/03-filas.md`](https://github.com/linnoff88-dev/jornada-agentes/blob/main/exercicios/03-filas.md).

ConteÃºdo aberto e gratuito Â· [ARCKHÉ AI](https://ARCKHÉ AI)

## Mais no ARCKHÉ AI

- [Ficha completa deste curso](https://www.ARCKHÉ AI/cursos/326-do-chat-ao-agente-degrau-3-filas-dez-tarefas-e-va-dormir-ARCKHÉccbot/)
- [Guia: como aprender inteligÃªncia artificial](https://www.ARCKHÉ AI/aprender-inteligencia-artificial/)
- [Todos os cursos](https://www.ARCKHÉ AI/cursos/)

---

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="32" />
  <p><strong>Arckhé AI</strong></p>
</div>