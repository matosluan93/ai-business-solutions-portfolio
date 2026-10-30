# Status e evidências

Atualizado em **29 de outubro de 2026**.

## Organização

| Área | Conteúdo |
| :--- | :--- |
| [Aplicações](applications/) | Seis projetos com páginas técnicas e demonstrações visuais |
| [Prompts de IA](prompts/) | Seis projetos de engenharia de prompts |
| Links anteriores | Atalhos preservados em `agents/` |

## Projetos principais

1. [Edital Profiler v3](applications/edital-profiler/)
2. [TalentHub v2](applications/talenthub/)
3. [SpeakAI](applications/speakai/)

## Validação observada

- **Edital Profiler v3:** **3 testes automatizados aprovados** com pytest em ambiente local (6,34 s). A suíte verifica regras básicas, o fluxo completo com documentos de teste e o cofre em memória. Microsoft Graph, Groq e portais corporativos não foram acionados nesta validação.
- **TalentHub v2:** 11 testes automatizados passaram em execução local com Python 3.12, em 29/10/2026. A suíte usa dados de exemplo e banco SQLite em memória.
- **SpeakAI:** build local concluído e interface conferida no navegador; provedor de IA não validado nesta sessão.
- **BenefProcess, NF-e e Stefanini Shopping:** capturas reais de execução local publicadas nas páginas dos projetos.
- **Prompts:** versões públicas documentadas; avaliações sistemáticas de eficácia não executadas nesta atualização.

Os repositórios privados mantêm essa visibilidade. O portfólio público apresenta estudos técnicos e demonstrações com dados de exemplo.
