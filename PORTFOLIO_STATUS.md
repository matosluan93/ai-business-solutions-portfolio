# Status e evidências

Atualizado em **2 de novembro de 2026**.

## Organização

| Área | Conteúdo |
| :--- | :--- |
| Repositórios públicos próprios | 8, sem forks; inclui o perfil e o repositório do portfólio |
| Projetos principais | 4: Edital Profiler, TalentHub, SpeakAI e Atlas Naval |
| [Aplicações](applications/) | 7 projetos com páginas técnicas; 6 com demonstrações visuais |
| [Prompts de IA](prompts/) | 6 projetos de engenharia de prompts |
| Testes com aprovação documentada | 14: 11 do TalentHub e 3 do Edital Profiler |
| Links anteriores | Atalhos preservados em `agents/` |

## Projetos principais

1. [Edital Profiler](applications/edital-profiler/)
2. [TalentHub](applications/talenthub/)
3. [SpeakAI](applications/speakai/)
4. [Atlas Naval](applications/atlas-naval/)

## Validação observada

- **Edital Profiler:** **3 testes automatizados aprovados** com pytest em ambiente local (6,34 s). A suíte verifica regras básicas, o fluxo completo com documentos de teste e o cofre em memória. Microsoft Graph, Groq e portais corporativos não foram acionados nesta validação.
- **TalentHub:** 11 testes automatizados passaram em execução local com Python 3.12, em 29/10/2026. A suíte usa dados de exemplo e banco SQLite em memória.
- **SpeakAI:** build local concluído e interface conferida no navegador; provedor de IA não validado nesta sessão.
- **BenefProcess, NF-e e Stefanini Shopping:** capturas reais de execução local publicadas nas páginas dos projetos.
- **Atlas Naval:** código público; sintaxe JavaScript, arquivos JSON e estrutura dos 19 estudos (IDs, coordenadas, fases e respostas dos quizzes) verificados em 02/11/2026. Capturas de tela e validação da interação visual pendentes.
- **Prompts:** versões públicas documentadas; avaliações sistemáticas de eficácia não executadas nesta atualização.

Os totais foram conferidos em **02/11/2026** com a lista de repositórios e as pastas de projetos publicadas. A contagem de testes consolida as aprovações já registradas acima; não houve nova execução das suítes nesta atualização.

Os repositórios privados mantêm essa visibilidade. O portfólio público apresenta estudos técnicos e demonstrações com dados de exemplo.
