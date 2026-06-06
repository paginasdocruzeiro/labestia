LaBestia, pacote produto vNext

Arquivos para subir no GitHub Pages:
- index.html
- assets/ (CSS, JS e imagens)
- data/ (bases em JSON: players, opponents, formations)
- .nojekyll (opcional, recomendado)

Observação: como as bases agora estão em data/*.json, abrir o index.html diretamente por file:// pode ser bloqueado pelo navegador. No GitHub Pages funciona normalmente. Para testar localmente, use um servidor simples, por exemplo:
python -m http.server 8000
