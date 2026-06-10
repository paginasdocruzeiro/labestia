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


Patch Elifoot banco:
- Modo Elifoot agora permite escolher 7 suplentes antes da Libertadores.
- No intervalo, até 3 suplentes podem ser acionados para influenciar o segundo tempo.
- Base de jogadores atualizada com Valdo, Djair, Rivaldo, Edmundo, Rincón, Élber, Renato Gaúcho, Deivid e Jussiê.
- Ricardo Goulart, Sorín e Nonato ajustados para overall 95.


Correção desta versão
- Corrigido o botão do Modo Elifoot antes da partida. O ecrã de plano inicial chamava uma função antiga inexistente (`dossierHtml`), o que travava o clique em “Jogar partida”.
- Validado fluxo Elifoot: abrir jogo, iniciar plano, intervalo, usar banco, terminar partida e avançar rodada.


Atualização Elifoot Tempos + Gestão de Equipa:
- O Modo Elifoot agora tem velocidades 1x, 2x, 3x e Imediato.
- Primeiro e segundo tempos passam a ser revelados em eventos, não instantaneamente.
- Adicionada tela Montar equipa para trocar titulares e reservas no Modo Elifoot.


Atualização mercado sem reroll:
- Propostas da diretoria agora são fechadas.
- Ao receber 3 opções, o jogador deve aceitar uma troca ou manter o titular.
- Não há botão Voltar para gerar novas propostas para o mesmo jogador.


Atualização Final Continental:
- data/final_venues.json guarda as sedes possíveis da final.
- A sede é sorteada quando LaBestia chega à final.
- CSS recebeu uma camada de limpeza visual para reduzir ruído sem alterar a identidade.


Versão corrigida: a sede da final aparece na tela do mata-mata, na tela pré-jogo, durante a partida e no resumo final. O ficheiro data/final_venues.json deve estar no GitHub junto com os restantes JSONs.

Patch Mundial PSG
- Adicionado data/psg_world.json com elenco atual do PSG 2025/26.
- Após conquistar a Libertadores, o jogador recebe o convite para disputar a final do Mundial contra o Paris Saint-Germain.
- PSG tem rating 95 e XI inicial com média exata 95.
- A final mundial é opcional: é possível jogar ou encerrar a campanha como campeão da Libertadores.
- O Mundial funciona no Modo Clássico e no Modo Elifoot, com pênaltis em caso de empate.
- Novas conquistas: O Mundo é Azul e Desafiou a Europa.

Patch Remodelação Abas + Legado
- Interface reorganizada em Draft, Revisão da Besta, Campanha por abas e Legado.
- Campanha agora usa abas: Jogo, Elenco, Dados e História.
- Revisão pré-campanha usa abas: Resumo, Titulares, Identidade e Detalhes.
- Topo simplificado com Menu para ações secundárias.
- Legado local: conta campanhas, Libertadores, Mundiais e melhor pontuação.
- O contador de títulos parte das duas Libertadores reais do Cruzeiro, então a primeira conquista no jogo é Tri, depois Tetra, Penta, Hexa, etc.
- Formations.json ampliado para 15 formações táticas, adaptadas às posições do jogo.

Patch Pedrinho Galáctico:
- Evento secreto antes da final do Mundial, somente se o jogador aceitar enfrentar o PSG.
- Exige três titulares elegíveis com OVR 86+ nas posições ATA, MEI, PE, PD ou ZG, com compatibilidade para Messi, Cristiano Ronaldo e Van Dijk.
- Decisão irreversível: aceitar a aposta obriga a escolher três jogadores para sair.
- 50% de chance de Messi, Cristiano Ronaldo e Van Dijk chegarem com OVR 99.
- 50% de chance de eles "bebetarem" e chegarem com OVR 79.
- Messi: ATA/PD/MEI. Cristiano Ronaldo: PE/PD/ATA. Van Dijk: ZG.

Patch Reequilíbrio + Modo Especialista de Cruzeiro:
- Antes do primeiro sorteio, o jogador escolhe Modo Normal ou Modo Especialista.
- No Modo Especialista, overalls e ratings de adversários ficam ocultos durante draft e campanha, substituídos por faixas como Forte, Assustador e Lendário.
- As notas continuam existindo internamente e são reveladas no resumo final.
- Legado agora registra conquistas no Especialista separadamente.
- Novas conquistas: Especialista da América e Especialista do Mundo.
- Fase de grupos e mata-mata ficaram mais difíceis.
- Improvisações, time torto e desequilíbrio pesam mais.
- Características continuam influenciando, mas com menos bônus puro por acúmulo.
- Mercado agora reduz moral em -2 por contratação, para simular impacto no grupo.
- PSG e fases decisivas receberam ajuste de dificuldade.
