# Status e evidências

Atualizado em **5 de novembro de 2026**.

## Organização

| Área | Conteúdo |
| :--- | :--- |
| Repositórios públicos próprios | 8, sem forks; inclui o perfil e o repositório do portfólio |
| Projetos principais | 4: Edital Profiler, TalentHub, SpeakAI e Atlas Naval |
| [Aplicações](applications/) | 7 projetos com páginas técnicas; 6 com demonstrações visuais |
| [Prompts de IA](prompts/) | 6 projetos de engenharia de prompts |
| Testes pytest aprovados | 20 (17 do TalentHub e 3 do Edital Profiler) |
| Links anteriores | Atalhos preservados em `agents/` |

## Projetos principais

1. [Edital Profiler](applications/edital-profiler/)
2. [TalentHub](applications/talenthub/)
3. [SpeakAI](applications/speakai/)
4. [Atlas Naval](applications/atlas-naval/)

## Validação observada

- **Edital Profiler:** **3 testes aprovados** em 05/11/2026, com regras documentais, fluxo local e cofre em memória. [Resultados](applications/edital-profiler/#evidência-de-testes)
- **TalentHub:** em 05/11/2026, a execução local com SQLite em memória e dados fictícios registrou **17 aprovações e 4 falhas conhecidas**. A avaliação incluiu 10 cenários do assistente de políticas. [Detalhes e resultados](applications/talenthub/#avaliação-do-assistente-de-políticas)
- **SpeakAI:** build com 8 cursos, navegação e tutores no Chromium, com teste local do chat usando Anthropic simulada. [Resultados](applications/speakai/#evidência-de-testes)
- **BenefProcess:** importação, regras de elegibilidade, XLSX, CSV e auditoria com dados fictícios. [Resultados](applications/benefprocess/#evidência-de-testes)
- **NF-e:** autenticação, validação e mudanças de estado no SQLite temporário. [Resultados](applications/nfe-automation/#evidência-de-testes)
- **Stefanini Shopping:** TypeScript, catálogo e persistência verificados. Contador do cabeçalho desatualizado após adicionar item. [Resultados](applications/stefanini-shopping/#evidência-de-testes)
- **Atlas Naval:** sintaxe, dados de 19 estudos e API local com indisponibilidade externa simulada. [Resultados](applications/atlas-naval/#evidência-de-testes)
- **Prompts:** versões públicas documentadas; avaliações sistemáticas de eficácia não executadas nesta atualização.

Os totais de repositórios e projetos refletem a conferência de **02/11/2026**. A contagem de testes pytest incorpora as execuções locais de TalentHub e Edital Profiler em **05/11/2026**. As verificações dos outros projetos são descritas separadamente por fluxo.

Os repositórios privados mantêm essa visibilidade. O portfólio público apresenta estudos técnicos e demonstrações com dados de exemplo.
