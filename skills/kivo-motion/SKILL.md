---
name: kivo-motion
description: Criar motions HyperFrames com hierarquia, timing e movimento relacionados ao conteúdo.
---

# kivo-motion

Prioridade: pedido atual e correções explícitas, decisões deste projeto, regras da casa, hábitos observados e, por último, esta skill. A identidade vem do kit atual. Não transforme um teste em gosto geral nem transporte cores, fontes ou decisões entre marcas.

Leia get_motion_guide antes de usar a API do KIVO. Use GSAP com timeline pausada em window.__timelines e duração igual ao trecho. Garanta que fontes carregaram e que buscar um tempo específico produz o mesmo quadro.
Desenhe primeiro a composição estática. Depois estabeleça ordem de atenção: entrada, leitura, saída. Não anime todos os elementos com a mesma intensidade ao mesmo tempo.
Escolha easing pelo comportamento: desaceleração para chegada, aceleração para saída, linear para fluxo contínuo. Back/elastic são recursos expressivos, não padrão para logos clínicos. Confira a curva na documentação/visualizador do GSAP.
Sincronize a ênfase com a palavra ou gesto relevante; música é outro apoio, não uma obrigação de cortar em toda batida. Ajuste tempo de leitura ao texto real, com pausa estável quando ajudar.
Crie movimentos que expliquem: conexão, fluxo, comparação ou percurso. Diagramas médicos devem ser esquemáticos e baseados no conteúdo fornecido, sem simular comprovação científica.
Evite reutilizar em todas as cenas a sequência cartão + blur + linha + partículas. Escolha uma família coerente e varie de acordo com a função.
Faça check_motion em entrada, leitura e saída para detectar cortes e sobreposição. Para avaliar fluidez, reproduza o trecho completo; não declare essa validação concluída apenas com screenshots.
Fontes: [GSAP Easing](https://gsap.com/docs/v3/Eases/) e [IBM — princípios de animação](https://www.ibm.com/design/language/animation/classic-principles/). A aplicação ao KIVO acima é uma adaptação editorial, não uma exigência dessas fontes.
