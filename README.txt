LaBestia Produto vNext + Mercado & Moral

Como publicar no GitHub Pages:
1. Suba todos os ficheiros e pastas deste pacote para a raiz do repositório.
2. Mantenha a estrutura:
   index.html
   .nojekyll
   assets/labestia.css
   assets/labestia.js
   assets/*.png
   data/players.json
   data/opponents.json
   data/formations.json
3. Em Settings > Pages, use Deploy from a branch, main, /(root).

Como testar localmente:
python -m http.server 8000
Depois abra http://localhost:8000

Novidades desta versão:
- Janela de contratações antes das oitavas.
- A diretoria libera aleatoriamente 1, 2 ou 3 contratações.
- Para cada jogador substituído, aparecem 3 opções da mesma posição.
- Moral da Besta começa em 80.
- Vitórias sobem moral em +5, goleadas em +8.
- Derrotas derrubam moral em -5, goleadas em -8.
- Eventos aleatórios de vestiário têm 10% de chance antes de cada jogo.
- Moral influencia levemente ataque e defesa na simulação.
