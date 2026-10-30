# Ferramentas, tecnologias e conhecimentos

Inventário baseado no código, nas dependências e nos materiais dos seis projetos de aplicação e dos seis projetos de prompts. As páginas de cada projeto indicam o estágio de implementação e a validação observada.

## Por projeto

| Projeto | Stack principal | Conhecimentos demonstrados |
| :--- | :--- | :--- |
| [Edital Profiler v3](applications/edital-profiler/) | Python, Flask, SQLAlchemy, SQLite, NumPy, Playwright, MSAL | Processamento documental, recuperação de contexto, critérios de comparação, organização de arquivos e automação em etapas |
| [TalentHub v2](applications/talenthub/) | Python, Flask, SQLAlchemy, SQLite, MSAL, NumPy | API REST, CRUD, sessões, CSRF, permissões por perfil, indicadores e recuperação com fontes |
| [SpeakAI](applications/speakai/) | JavaScript, HTML, CSS, Node.js, Web Speech API, localStorage | Jornada de aprendizagem, gamificação, estado no navegador, internacionalização e endpoint de conversação |
| [BenefProcess](applications/benefprocess/) | Python, Flask, pandas, openpyxl, xlsxwriter, python-pptx | Validação, deduplicação, rastreabilidade, regras de transformação e geração de entregáveis |
| [Stefanini Shopping](applications/stefanini-shopping/) | Next.js, React, TypeScript, Tailwind CSS, Lucide React | Interface responsiva, catálogo, variantes, carrinho, UX e internacionalização |
| [NF-e — Automação](applications/nfe-automation/) | Python, Flask, SQLite, HTML, CSS, JavaScript | Persistência local, cadastro, consulta, painel e pré-visualização de documentos |

## Linguagens e desenvolvimento

- **Linguagens:** Python, JavaScript e TypeScript; HTML e CSS para estrutura e apresentação.
- **Backend:** Flask, Flask-SQLAlchemy, SQLite, APIs REST, requests, python-dotenv e Waitress.
- **Front-end:** React, Next.js, Tailwind CSS, Lucide React, JSON local e recursos nativos do navegador.
- **Estado e experiência:** localStorage, Web Speech API, temas, responsividade e internacionalização.

## Dados e documentos

- **Planilhas e dados tabulares:** pandas, openpyxl, xlsxwriter, xlrd e python-calamine, conforme as dependências do BenefProcess.
- **PDF e Word:** pdfplumber, pypdf e python-docx no processamento de documentos.
- **Apresentações e estrutura documental:** python-pptx e lxml no BenefProcess.
- **Persistência e modelagem:** SQLite e ORM SQLAlchemy em aplicações locais.
- **Operações:** validação de registros, deduplicação, classificação de arquivos, normalização de texto, auditoria e exportação de relatórios.

## IA, busca e automação

- **Engenharia de prompts:** hierarquia de instruções, contexto, formato de resposta, critérios e limites de uso.
- **Recuperação de contexto:** divisão de texto em trechos, indexação local, vetores por hashing de termos com NumPy, similaridade e apresentação de fontes.
- **APIs de modelos presentes no código:** Groq no Edital Profiler, Azure OpenAI como opção no TalentHub e Anthropic no endpoint do SpeakAI. As chamadas dependem da configuração de cada ambiente; a presença do código não comprova homologação externa.
- **RPA:** Playwright, seletores configuráveis, orquestração por etapas e tratamento de pendências. Os roteiros de portais têm limites de implementação declarados no Edital Profiler.

## Integrações e bibliotecas preparadas

| Integração | Projeto | Estágio documentado |
| :--- | :--- | :--- |
| Microsoft Entra ID / MSAL | TalentHub | Implementação configurável; testes de resolução de usuários sem homologação no tenant corporativo |
| Microsoft Graph / OneDrive | Edital Profiler | Implementação configurável; fluxo verificado em armazenamento local |
| keyring / cofre de credenciais | Edital Profiler | Integração implementada; teste com backend em memória |
| Supabase: supabase-js e SSR | Stefanini Shopping | Clientes e estruturas presentes; execução demonstrada com catálogo local |
| Bling / OAuth e REST | NF-e — Automação | Módulo presente no código; demonstração sem conexão com o serviço |
| Vercel / função Node.js | SpeakAI | Configuração e endpoint presentes; build local verificado |

## Projetos de prompts e conhecimentos de negócio

| Projeto | Conhecimentos aplicados |
| :--- | :--- |
| [Gestor Acolhe](prompts/gestor-acolhe/) | Apoio à liderança, governança e encaminhamento para revisão humana |
| [Sophie Voice Comms](prompts/sophie-voice-comms/) | Roteiros institucionais, localização e controle de informações |
| [SmartComms](prompts/smartcomms/) | Comunicação corporativa em inglês, UX writing e adaptação por canal |
| [SpeakAI — prompt](prompts/speakai/) | Tutoria de idiomas, personalização e desenho de jornadas |
| [LexAnalyzer](prompts/lexanalyzer/) | Estruturação preliminar de informações e explicabilidade; versão pública sanitizada |
| [SkillMatch](prompts/skillmatch/) | Critérios de comparação entre currículo e vaga e organização de evidências |

## Qualidade, colaboração e entrega

- **Git e GitHub:** versionamento, histórico, branches de arquivo e documentação de projetos.
- **pytest:** testes locais de autenticação, permissões, CRUD e fluxo de aplicação, conforme as suítes existentes.
- **ReportLab e python-docx:** geração de documentos de teste na suíte do Edital Profiler.
- **Documentação:** Markdown, escopo, limitações, evidências de execução e demonstrações visuais.
- **Análise de negócios:** levantamento de requisitos, regras operacionais, organização de processos e rastreabilidade das entregas.

[Status e resultados observados](PORTFOLIO_STATUS.md) · [Mapa de projetos](PROJECTS.md) · [Portfólio](README.md)
