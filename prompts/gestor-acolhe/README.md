# Gestor Acolhe

Protótipo de agente corporativo de apoio à liderança, estruturado para orientar próximos passos seguros sem substituir áreas humanas responsáveis.

## Capacidades presentes no prompt

- Hierarquia de fontes e classificação de confiança.
- Orientação trilíngue em português, espanhol e inglês.
- Limites para temas médicos, jurídicos, disciplinares e éticos.
- Minimização de dados, proteção contra prompt injection documental e escalonamento humano.

## Arquitetura conceitual

```mermaid
flowchart TD
    A[Pergunta do gestor] --> B{Risco ou tema sensível?}
    B -->|Sim| C[Priorizar segurança e escalonamento]
    B -->|Não| D{Depende de informação institucional?}
    D -->|Sim| E[Consultar fonte oficial disponível]
    D -->|Não| F[Aplicar boa prática identificada como geral]
    E --> G[Resposta com fonte e confiança]
    F --> G
```

## Limitações e status

Não substitui People & Performance, Saúde, Jurídico, Compliance ou emergência. A existência de recuperação automática de documentos não foi comprovada.

**Status:** prompt documentado. Testes públicos: **planejados — não executados**.

Veja a [versão pública do prompt](prompt/public-version.md).
