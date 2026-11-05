# Atlas Naval

## História naval em um globo 3D interativo

Aplicação educacional em português para explorar batalhas navais pela localização geográfica, entender sua evolução tática e revisar o conteúdo. Inclui material para o estudo de Fuzileiros Navais e para interessados em história militar.

[Código público e documentação](https://github.com/matosluan93/atlas-naval) · [Abrir aplicação](https://carta-de-combate-naval.vercel.app) · [Estudo de Riachuelo](https://carta-de-combate-naval.vercel.app/#b-riachuelo)

## O que o projeto demonstra

- **Visualização geográfica:** globo CesiumJS, imagens de satélite, marcadores e controle de câmera.
- **Aprendizagem interativa:** 19 estudos completos com fichas, animações por fases, lições, papel dos fuzileiros e quizzes.
- **Busca e filtros:** batalha, guerra, ano, Brasil, operações anfíbias e época.
- **Integração de dados:** API Node.js que coleta, enriquece e deduplica registros de fontes públicas.
- **Revisão e persistência:** modo treino e resultados guardados no navegador com `localStorage`.
- **Interface responsiva:** layout adaptado a computador e celular.

## Tecnologias

**JavaScript · HTML · CSS · CesiumJS 1.139.1 · Node.js · Vercel Functions · SheetJS (`xlsx`) · SPARQL**

## Arquitetura

O navegador reúne os estudos incluídos no código com o catálogo servido por `/api/batalhas`. A função consulta Wikidata, Wikipedia, The War Atlas, NAVBATTLE, American Civil War Battle Data e MAREA. Depois normaliza os registros, remove duplicatas e complementa metadados. O total do catálogo varia conforme a disponibilidade dessas fontes.

O globo funciona sem token do Cesium ion; o relevo 3D é opcional. A execução completa da API usa funções da Vercel, enquanto o front-end não exige compilação.

## Evidência de testes

Em **5 de novembro de 2026**, as verificações locais em Node.js confirmaram:

- Sintaxe de **6 scripts JavaScript** e leitura de **4 arquivos JSON**.
- **19 estudos** com identificadores únicos, coordenadas válidas, fases descritas, trajetórias e índices de respostas dos quizzes dentro das opções disponíveis.
- A rota `/api/batalhas` retornou **HTTP 200 e 48 registros locais** quando a rede externa foi simulada como indisponível. O modo de diagnóstico registrou a indisponibilidade da Wikidata e usou cabeçalho `no-store`.

O teste da rota foi feito com respostas externas simuladas como indisponíveis. A renderização do globo e a coleta real das fontes ficaram fora da execução.

## Explorar

Consulte o [README do projeto](https://github.com/matosluan93/atlas-naval#readme) para instruções de execução local, publicação na Vercel, estrutura de arquivos e atribuições das fontes.

[Voltar às aplicações](../README.md) · [Voltar ao portfólio](../../README.md)
