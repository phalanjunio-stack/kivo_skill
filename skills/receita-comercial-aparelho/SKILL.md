---
name: receita-comercial-aparelho
description: Receita de storyboard para comercial de equipamento estético sem locução (só música e textos), no estilo do reel FoLix — planos-herói do aparelho, cortes na batida, tipografia editorial e revelação da marca no fim.
---

# Receita · Comercial de aparelho (sem fala)

Referência principal: reel do FoLix (Lumenis) — fundo preto, aparelho com anel de luz da cor da marca, macro da ponteira, corte de pele em CGI, selos de certificação, textos pequenos à esquerda com uma palavra em destaque. O que faz ele ser bonito é o **material** (planos-herói limpos, luz de estúdio); a edição em cima é simples e precisa.

## 0. Antes de montar: os planos-herói
- Liste o que existe na Mídia e olhe cada um (get_media_frames). Precisa de pelo menos 4 planos-herói: aparelho inteiro com luz, detalhe/macro da ponteira, aplicação ou tela, e um plano de efeito (pele, energia, CGI).
- O que faltar: gere no Spaces a partir da foto real do aparelho (imagem → vídeo), um plano por vez, e **mostre à pessoa antes de seguir**. Sem planos-herói bons, não monte: avise o que falta.
- Fotos e vídeos de WhatsApp, baixa resolução ou com bastidor não entram como plano principal.

## 1. Estrutura (25–45 s, nas batidas fortes da música)
| Bloco | Duração | Plano | Texto |
|---|---|---|---|
| Revelação | 2–3 s | aparelho no escuro, luz revelando | `palavra_gigante` com o nome da tecnologia |
| Produto | 6–10 s | aparelho inteiro, câmera orbitando | 1 `escrita_palavras` curta |
| Tecnologia | 8–12 s | macro da ponteira + efeito na pele | 2 `destaque_fala` (por cima, sem pessoa: use como título) |
| Drop | 3–4 s | cortes de 0,5 s entre os planos-herói | sem texto |
| Prova | 3–5 s | selos/certificações reais do material | `escrita_palavras` com o selo |
| Assinatura | 3–3,5 s | fundo escuro | `revelacao_logo` com a logo oficial |

## 2. Ritmo e transições
- Todo corte numa batida forte (kit.music.down). Planos lentos (2 batidas) no começo, cortes a cada batida no drop.
- Transições no máximo 5 tipos no vídeo: `passagemluz` (revelação), `whipleft`/`whipright` (energia), `flash` 0,2 s (entrada do drop), `desfoquelente` (antes do logo), corte seco no resto.
- Curvas de velocidade só no drop (`whipCut`) e no primeiro plano do aparelho (`reveal`).

## 3. Texto
- No máximo 7 cartelas no vídeo inteiro. Frase de 2–7 palavras. Uma palavra em destaque por cartela.
- Textos na metade de baixo ou à esquerda, nunca sobre o aparelho (confira com get_frames).
- Só alegações que estão no material da marca (registro ANVISA, FDA, frequência, número de eletrodos). Nada de "sem dor", "resultado garantido".

## 4. Som e cor
- Música do kit, fade final, −14 LUFS. Áudio dos clipes mudo.
- Cor: pretos profundos, contraste +10, um look para o vídeo inteiro (o mesmo em 3D, IA e filmagem).
