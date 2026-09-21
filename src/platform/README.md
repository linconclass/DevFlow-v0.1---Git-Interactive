# Product Platform

Esta pasta define contratos do produto sem acoplar a UI a um fornecedor específico.

- `types.ts`: domínio de usuário, plano e progresso.
- `progress.ts`: interface de persistência + adapter local atual. Futuro backend substitui o adapter sem alterar os módulos.
- `entitlements.ts`: capacidades Free, Pro e Education.

Próximas implementações privadas: autenticação, persistência cloud, analytics, billing e classroom.
