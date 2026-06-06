LaBestia Performance Pack

Abra index.html depois de extrair o ZIP.

Optimizações aplicadas:
- CSS e JavaScript separados para melhor cache e carregamento.
- Imagens base64 externalizadas em assets/.
- Modo leve para reduzir animações, sombras e efeitos pesados.
- Placar ao vivo optimizado: actualiza apenas score, minuto e eventos, sem reconstruir a tela inteira a cada tick.
- Cache de encaixe por jogador/posição para reduzir cálculos repetidos no draft.
- Seleção de carta com renderização parcial, evitando renderAll desnecessário.
- Suporte a prefers-reduced-motion.

Ficheiros principais:
- index.html
- assets/labestia.css
- assets/labestia.js
- assets/*.png
