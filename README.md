# Filas: dez tarefas e vêÂ¡ dormir ê¢â¬â curso (ARCKHê Learning v7.2)

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="48" />
  <p><strong>Arckhé AI</strong></p>
</div>


Curso completo do **degrau 3** da formaêÂ§êÂ£o [Do chat ao agente](https://linnoff88-dev.github.io/ mandar vêÂ¡rias tarefas para uma fila durêÂ¡vel, sair de perto e encontrar o trabalho feito, com portêÂ£o onde precisa de vocêÂª. A ferramenta êÂ© o [ARCKHêccbot](https://linnoff88-dev.github.io/ (gateway do Telegram + fila durêÂ¡vel).

**Abrir o curso:** https://linnoff88-dev.github.io/

**Other languages:** [English](https://linnoff88-dev.github.io/ êÂ· [EspaêÂ±ol](https://linnoff88-dev.github.io/

## As 7 aulas

1. **Do chat êÂ  fila** ê¢â¬â as quatro garantias de uma fila durêÂ¡vel.
2. **O que vai para a fila** ê¢â¬â triagem em sozinha, com portêÂ£o ou fica com vocêÂª.
3. **A fila caseira em 30 linhas** ê¢â¬â `fila-caseira.sh`, interromper e retomar (simulaêÂ§êÂ£o).
4. **Instalar o ARCKHêccbot** ê¢â¬â atêÂ© o `/ping` responder; pareamento e segredos.
5. **Mandar o lote** ê¢â¬â skills, as cinco filas, `/fila`, `/jobs`, cêÂ³digo 143.
6. **PortêÂµes** ê¢â¬â fluxo com portêÂ£o, `/pronto`, reprovar com correêÂ§êÂ£o, `| sombra` (simulaêÂ§êÂ£o).
7. **O dia seguinte** ê¢â¬â conferir, medir as certas na primeira, regra nova e plano com datas.

## Como funciona

| Arquivo | O que êÂ© |
|---|---|
| `conteudo/pt/curso.json` | nome, vêÂ­deos, pêÂ¡gina inicial e textos da interface |
| `conteudo/pt/aulas/*.json` | uma aula por arquivo |
| `gerar.py` | monta `index.html` e `aulas/<slug>/index.html` |
| `validar.py` | portêÂ£o de qualidade (`--links` confere os links externos) |
| `assets/` | CSS, JS, imagens e legendas (`filas.js`/`filas.css`: simulaêÂ§êÂ£o do portêÂ£o) |

```bash
python3 gerar.py && python3 validar.py --links
```

EN e ES (`en/`, `es/`): textos em `conteudo/en|es/`, gerados por `traduzir.py` da skill (Codex da assinatura, cache em `i18n/`); capa com texto em `assets/img/capa-en.jpg` e `capa-es.jpg`.

```bash
python3 ~/.claude/skills/formato-curso-v72/scripts/traduzir.py . en es
python3 gerar.py --lang en && python3 gerar.py --lang es
python3 validar.py --lang en && python3 validar.py --lang es
```

HTML estêÂ¡tico, sem build e sem backend. O progresso fica sêÂ³ no navegador de quem estuda.

VêÂ­deos da sêÂ©rie *Do chat ao agente* ([jornada-agentes](https://github.com/linnoff88-dev/jornada-agentes), release `video-v2.0.0`). ExercêÂ­cios originais em [`exercicios/03-filas.md`](https://github.com/linnoff88-dev/jornada-agentes/blob/main/exercicios/03-filas.md).

ConteêÂºdo aberto e gratuito êÂ· [ARCKHê AI](https://ARCKHê AI)

## Mais no ARCKHê AI

- [Ficha completa deste curso](https://www.ARCKHê AI/cursos/326-do-chat-ao-agente-degrau-3-filas-dez-tarefas-e-va-dormir-ARCKHêccbot/)
- [Guia: como aprender inteligêÂªncia artificial](https://www.ARCKHê AI/aprender-inteligencia-artificial/)
- [Todos os cursos](https://www.ARCKHê AI/cursos/)

---

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="32" />
  <p><strong>Arckhé AI</strong></p>
</div>