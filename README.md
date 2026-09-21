# DevFlow — Engenharia de Software Visual

DevFlow é uma experiência **mobile-first** para aprender Engenharia de Software vendo o estado dos sistemas mudar, em vez de depender apenas de texto e cheatsheets.

## Estado atual — v0.6

A base evoluiu de um laboratório isolado de Git para uma plataforma multi-módulo.

### Experiências interativas
- Git Fundamentals: Working Directory → Staging → Commit → Remote
- Branches & Merge: árvore visual, divergência, merge e conflito
- Git Challenges: decisões baseadas em cenários com feedback
- Learning Map pesquisável
- Visual Lessons reutilizáveis
- Progresso persistido localmente
- PWA com service worker e suporte offline básico

### Módulos disponíveis no Learning Map
- **Git** — fundamentos, histórico, branches, merge, remotes, reset/revert, stash, rebase, cherry-pick e gitignore
- **Java** — JVM, OOP, Stack/Heap, Collections, Streams e Exceptions
- **Spring Boot** — Bean Lifecycle, DI, REST Controller, JPA e Security
- **SQL & Database** — SELECT, JOIN, índices, transações e modelagem
- **APIs & Web** — HTTP, REST, status codes, JWT, CORS e WebSocket

Cada conceito segue a mesma estrutura: **entender → visualizar → ver exemplo → responder desafio → concluir**.

## Stack
React · TypeScript · Vite · localStorage · Service Worker

## Executando
```bash
npm install
npm run dev
```

## Arquitetura
```
src/
├── App.tsx             # shell e navegação
├── content.ts          # catálogo de módulos e conceitos
├── LearningHub.tsx     # engine reutilizável de trilhas/aulas
├── BranchLab.tsx       # laboratório visual de branches
├── ChallengeLab.tsx    # engine inicial de desafios
└── *.css               # estilos por experiência

public/
├── manifest.webmanifest
└── sw.js
```

## Roadmap
A plataforma já possui a fundação dos módulos até **APIs & Web**. Próximas evoluções: aprofundar laboratórios de Java/Spring/SQL/API, sistema global de XP/conquistas, testes automatizados, acessibilidade, PWA completa com ícones e publicação.

---
Projeto de portfólio desenvolvido por Lincon Class.
