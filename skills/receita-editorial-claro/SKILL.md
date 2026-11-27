---
name: receita-editorial-claro
description: Receita de storyboard para campanha clínica premium em tema claro (nude, creme, champagne) — tipografia editorial em serif e sans grafite, destaque na cor da marca, brilhos discretos, como a arte do EuroPlasma e a referência vintage do Pinterest.
---

# Receita · Editorial claro (premium)

Referências: arte oficial EuroPlasma (fundo nude/champagne, "EuroPlasma" em sans grafite, frase de apoio em serif itálico, gota de brilho turquesa) e "Let this rip" no Pinterest (creme e preto, luz de janela, palavra gigante apagada ao fundo, brilhos de 4 pontas, objetos recortados).

Use quando o kit da marca é claro (paleta com nude, creme, champagne, branco) ou a demanda pede "premium", "elegante", "clínico".

## Regras visuais
- Fundo das cenas de texto: a cor mais clara do kit (ex.: #ece0d1). Texto: grafite do kit (ex.: #2f2f33). Destaque: a cor de acento do kit (ex.: turquesa #37c6bd → #1f9e96).
- Motions no tema claro: `palavra_gigante` com `tema: 'claro'`; `escrita_palavras` com `fundo: 'claro'`.
- Por cima de vídeo (pessoa falando), use `destaque_fala` normal (texto branco) — o tema claro é para as cenas de texto e o fechamento.
- Cor do vídeo: grade levemente quente (temperatura +8, saturação 95), para casar com o nude.
- Proibido neste estilo: HUD, glitch, RGB split, flash branco, whip. Transições: corte seco, `dissolve` 0,4 s, `desfoquelente` 0,35 s.

## Estrutura
1. **Abertura:** plano real mais bonito (macro do aparelho ou da aplicação) 2–3 s, com `palavra_gigante` tema claro *por cima de um card nude* ou `destaque_fala` se houver fala.
2. **Corpo:** receita-pessoa-falando (se houver fala) ou receita-so-texto (se não houver), trocando o tema para claro.
3. **Fechamento (3,5–4 s):** card no fundo claro do kit com a frase de assinatura em serif itálico (`escrita_palavras` com `fundo: 'claro'`, 1 `*destaque*`) e depois `revelacao_logo` com a logo oficial em versão escura e `assinatura` curta. Logo da empresa (ex.: Contourline em azul-marinho) pequena embaixo, íntegra.

## Conferência
- Toda logo na versão que contrasta com o fundo claro (versão escura/cinza). Logo branca sobre nude é erro.
- Texto grafite em cima de vídeo escuro some: confira com get_frames.
