# NF-e — Automação

Protótipo web local para organizar dados de notas e apresentar uma interface inspirada em DANFE para controle interno.

## Demonstração visual

Capturas reais do protótipo em execução local, em 29/10/2026, com banco novo e vazio. O ambiente utiliza uma empresa de demonstração e não está conectado ao Bling ou à SEFAZ. As telas não comprovam emissão fiscal oficial.

### Cadastro e pré-visualização

![Formulário de nota e área de pré-visualização do protótipo NF-e](01-formulario.jpg)

### Painel de acompanhamento

![Dashboard do protótipo NF-e com base de demonstração vazia](02-dashboard.jpg)

## Funcionalidades confirmadas na versão local inventariada

- Backend Flask.
- Persistência local em SQLite.
- Interface em HTML, CSS e JavaScript.
- Cadastro e consulta local de registros e produtos.
- Numeração local e visualização para impressão.

## Evidência de testes

Em **5 de novembro de 2026**, a API Flask foi exercitada com um SQLite temporário e emitente, destinatário e item fictícios.

- A API retornou HTTP 401 para acesso anônimo e para senha incorreta. O login de demonstração autenticou o cliente de teste.
- O cadastro sem itens retornou HTTP 400. Um rascunho válido foi gravado e recuperado com o item e a quantidade informada.
- O rascunho passou pelos estados locais de emissão e cancelamento, verificados por consulta ao registro no SQLite.

A verificação cobre a API do protótipo. Autorização fiscal e comunicação com Bling e SEFAZ ficaram fora da execução.

## Limitações críticas

Não há comprovação de integração produtiva com SEFAZ, certificado digital, assinatura oficial de XML, autorização fiscal ou emissão de NF-e com validade jurídica. O banco local foi retirado do rastreamento e protegido por `.gitignore`.

## Status

Protótipo funcional para uso e demonstração local, não emissor fiscal de produção.

Código: [matosluan93/nfe_system_v6](https://github.com/matosluan93/nfe_system_v6)

