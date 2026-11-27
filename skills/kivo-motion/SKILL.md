---
name: kivo-motion
description: Qual motion da biblioteca do KIVO usar para cada momento do vídeo, com os campos e as posições certas, e quando criar um HyperFrames novo.
---

# kivo-motion · qual motion usar

Primeiro a biblioteca (get_motion_library), depois criar do zero. Os modelos da biblioteca já têm fontes, zona segura, curvas e saída certas; um motion novo só quando nenhum serve.

## Os quatro do estilo das referências (27/11/2026)

| Momento | Modelo | Campos | Onde |
|---|---|---|---|
| Palavra-chave enquanto a pessoa fala | `destaque_fala` | `linha` (2–5 palavras ditas antes), `destaque` (a palavra), `apoio` (2–4 depois, opcional) | y 1060 (peito), por cima do vídeo |
| Frase de impacto / gancho / virada | `palavra_gigante` | `fundo` (1 palavra, caixa alta), `linha`, `destaque`, `tema` 'escuro' ou 'claro' | y 1020; em cena de texto, sobre fundo do kit |
| "Não é X, é Y", antes × agora, frase escrita | `escrita_palavras` | `frase` com `*destaque*` e `~riscada~`; `fundo` null (por cima do vídeo), 'escuro' ou 'claro' (cena só de texto) | y 900–1060 |
| Fechamento com a marca | `revelacao_logo` | `logo` (imagem) ou `nome`, `assinatura`, `fundo` | y 900 |

Todos aceitam `cor` = [r,g,b,r,g,b] de 0 a 1 (degradê das cores de destaque do kit) e `duracao`.

## Regras de uso
- Um motion por ideia; nunca dois ao mesmo tempo na tela.
- Entrada 0,1 s depois da palavra dita; duração até o fim da frase (mínimo 0,5 s + 0,3 s por palavra).
- Rosto e legenda livres: confira cada um com get_frames no meio da duração.
- Não use o mesmo modelo mais de 3 vezes seguidas; alterne `destaque_fala` com B-roll e respiro.
- Em comercial sem fala, `destaque_fala` funciona como título (por cima do plano do aparelho, sem pessoa).

## Criar um motion novo (só quando nenhum serve)
- get_motion_guide antes; create_motion; check_motion em entrada, leitura e saída.
- Siga o ofício do guia: chegada com cauda longa, saída 40–50% mais curta, título parado depois de chegar, palavras entrando com desfoque 6 px → 0 em 0,13 s.
- Desenho fotorrealista (pele, aparelho, CGI) não é motion: é Spaces (imagem/vídeo de IA).
