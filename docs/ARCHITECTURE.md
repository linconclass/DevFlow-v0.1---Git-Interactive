# DevFlow — Architecture Boundary

O DevFlow passa a ser tratado como produto, com separação explícita entre experiência pública/community e plataforma comercial.

## Camadas

### Community / Learning Content
Conteúdo educacional, conceitos e experiências que podem ser demonstrados publicamente.

### Learning Engine
Motor reutilizável de aulas, simulações, desafios e avaliação. A partir desta versão, novas capacidades estratégicas desta camada devem permanecer privadas.

### Product Platform
Autenticação, progresso em nuvem, gamificação global, analytics, billing, IA e recursos para instituições. Esta camada não pertence ao repositório community.

## Estrutura-alvo

```
src/
  app/          shell e navegação
  modules/      módulos educacionais
    git/
    java/
    spring/
    sql/
    api/
  shared/       UI e utilidades reutilizáveis
  platform/     somente contratos/adapters; implementação comercial privada
```

## Regra de produto
O repositório atual serve como base histórica/community do DevFlow. Novas funcionalidades comerciais não devem ser implementadas aqui automaticamente. A plataforma comercial deve evoluir em repositório privado próprio.
