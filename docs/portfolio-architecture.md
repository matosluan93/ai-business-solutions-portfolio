# Arquitetura do portfólio

O repositório central funciona como camada de apresentação. Aplicações com repositório próprio preservam seu histórico e recebem aqui apenas uma página técnica e um link.

```mermaid
flowchart TD
    P[Portfólio central] --> A[Agentes baseados em prompt]
    P --> B[Aplicações em repositórios próprios]
    A --> D[Documentação pública sanitizada]
    A --> E[Exemplos e testes sintéticos]
    B --> F[Resumo técnico e limitações]
    B --> G[Link para código original]
```
