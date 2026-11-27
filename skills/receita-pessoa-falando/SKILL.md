---
name: receita-pessoa-falando
description: Receita de storyboard para vídeo de pessoa falando (especialista, médica, depoimento) no estilo editorial dos Reels de referência — palavra-chave grande em serif itálico na altura do peito, cortes de B-roll no ritmo da fala e fechamento com a marca.
---

# Receita · Pessoa falando (estilo editorial)

Referências que definem o estilo (Pinterest, 27/11/2026): presets "CutPro" (palavra-chave dourada em serif itálico com palavras pequenas em volta), "Modern talking head" (antes/depois com destaque colorido e números grandes) e "Motion inspiration 2025" (legenda de uma palavra, linhas de luz). O que eles têm em comum e você deve reproduzir:

1. **A pessoa é a tela.** Rosto livre sempre. Todo texto fica no peito (y 1020–1300 no 9:16) ou acima da cabeça (y 220–420), nunca sobre o rosto.
2. **Uma palavra manda por vez.** Frase pequena em sans + a palavra que carrega o sentido GRANDE em serif itálico, com o degradê da marca e um brilho que passa uma vez.
3. **Ritmo de fala, não de efeito.** O destaque entra 0,1 s depois de a palavra ser dita e sai antes da próxima ideia.

## Passo a passo no KIVO

**Abertura (0–3 s) — gancho**
- Primeira frase forte da fala. Se houver B-roll impactante (aparelho ligando, macro da aplicação), ele cobre os 2 primeiros segundos por cima da voz, mudo.
- Motion: `palavra_gigante` com a ideia do vídeo (`fundo` = 1 palavra em caixa alta, `linha` = 3–5 palavras, `destaque` = 1–2 palavras). y 1020. Duração 2,6–3,2 s.

**Corpo — a cada 5 a 8 s, um destaque (no máximo 1 por frase e 6 por minuto)**
- Escolha na transcrição a palavra que é o *assunto* da frase (mecanismo, benefício real, nome da tecnologia). Nunca conectivos, nunca a frase inteira.
- Motion: `destaque_fala` com `linha` = 2–5 palavras ditas antes, `destaque` = a palavra-chave, `apoio` = 2–4 palavras ditas depois (ou vazio). y 1060. `start` = início da palavra − 0,1 s; duração = até o fim da frase (2,2–3,2 s).
- Contraste "não é X, é Y" ou correção na fala → `escrita_palavras` com `frase` = "Não é ~X~ É *Y*", por cima do vídeo (sem `fundo`), y 900–1060.
- Entre destaques: só legenda. Respiro é parte do estilo.

**B-roll — 30 a 45% do tempo**
- Explicação de mecanismo ou de procedimento → cubra com B-roll mudo (aplicação, tela do aparelho, detalhe), 2,5–4 s por plano, cortes no fim de frase ou de palavra forte.
- No ponto de ênfase, um punch-in no plano da pessoa: escala 1,00 → 1,12 em 0,3 s (keyframes com ease "out"), segura até o próximo corte. No máximo 1 a cada 10 s.
- Transições: corte seco na maioria; `whipleft`/`whipright` (0,25 s) só para entrar e sair de B-roll em momento de energia; `flash` (0,2 s) só no gancho.

**Legenda**
- Estilo salvo da casa (Contourline · Rolagem), 3 palavras por bloco, y 83. Ela sobe para não colidir quando houver motion no peito? Não: o motion fica em y 1020–1300 e a legenda em 83% — confira com get_frames; se encostar, suba o motion (y menor), nunca esconda a legenda.

**Fechamento (últimos 3–3,5 s)**
- `revelacao_logo` com `logo` = logo oficial do kit (ou `nome`), `assinatura` = nome do equipamento ou a chamada curta. `fundo: 'escuro'` sobre o último plano escurecido, ou um card no tema do kit.

**Som**
- Música na A2 com duck −12 dB sob a voz. Loudness final −14 LUFS.
- `whoosh` baixo (−18 dB) na entrada de cada `destaque_fala`/`palavra_gigante`. Nada de som em todo corte.

## Cores e fontes
- `cor` de todos os motions = degradê das duas cores de destaque do kit (de 0 a 1). Sem kit: dourado [1, 0.86, 0.5, 1, 0.52, 0.1].
- Fontes já estão nos modelos (Axiforma + Instrument Serif itálico). Não troque por fonte de sistema.

## Conferência antes de entregar
- get_frames no meio de cada destaque: rosto livre? legenda legível? palavra-chave inteira?
- Conte: no máximo 6 destaques por minuto; nenhum destaque repete a mesma palavra.
- A palavra destacada foi realmente dita naquele instante (get_transcript).
