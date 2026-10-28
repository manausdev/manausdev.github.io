# 📔 ADR Log — Registro Resumido de Decisões

Registro cronológico resumido (mais recente primeiro) das decisões de arquitetura
do projeto **ManausDev**. O índice completo, com mapa por feature e componente,
vive no [`README.md`](README.md).

| ADR | Data | Título | Status |
|:---:|:---:|:---|:---:|
| [0028](0028-alerta-dependabot-elliptic-cve-2025-14505.md) | 2026-10-28 | Alerta Dependabot de `elliptic` (CVE-2025-14505) — verificação e resolução | **Aceito** |
| [0027](0027-auditoria-acessibilidade-performance-e-ci.md) | 2026-10-20 | Auditoria de acessibilidade, performance e CI | **Aceito** |
| [0026](0026-reputacao-badges-moderacao-fase-5.md) | 2026-10-02 | Reputação, badges e moderação — Fase 5 do Community OS | *Proposto* |
| [0025](0025-materializar-grafo-ecossistema-como-produto.md) | 2026-10-02 | Materializar o grafo do ecossistema como produto | **Aceito** |
| [0024](0024-person-model-multiplos-papeis.md) | 2026-10-02 | Evoluir `profiles` para modelo Person com papéis múltiplos | *Proposto* |
| [0023](0023-generalizar-organizations-org-type.md) | 2026-10-02 | Generalizar Organizations com org_type incremental | *Proposto* |
| [0022](0022-svg-logo-header-light-dark-variants.md) | 2026-09-30 | SVG Logo no Header com variante clara (Pantone 2026 C) | **Aceito** |
| [0021](0021-community-os-domain-architecture-and-roadmap.md) | 2026-09-30 | Community OS — arquitetura orientada a domínios e roadmap | **Aceito** |
| [0020](0020-todo-reflects-verified-state.md) | 2026-09-30 | TODO.md reflete o estado verificado do código | **Aceito** |
| [0019](0019-favicon-from-brand-symbol.md) | 2026-09-30 | Favicon a partir do símbolo da marca | **Aceito** |
| [0018](0018-public-supabase-client-for-static-detail-routes.md) | 2026-09-30 | Cliente Supabase público para rotas de detalhe estáticas | **Aceito** |
| [0017](0017-css-modules-migration-icons-and-audit-findings.md) | 2026-09-29 | Migração para CSS Modules — ícones com `size`, chip de disponibilidade único e limites da auditoria | **Aceito** |
| [0016](0016-profile-types-and-permission-matrix.md) | 2026-09-29 | Tipos de perfil e matriz de permissões por tipo de conta | **Aceito** |
| [0015](0015-rebrand-blue-tech-palette-and-dark-mode.md) | 2026-09-29 | Rebrand para a paleta Blue-Tech com modo claro/escuro | **Aceito** |
| [0014](0014-fix-critical-nextjs-rce-and-remove-dead-middleware.md) | 2026-09-25 | Correção de RCE crítico no Next.js e remoção de Middleware morto | **Aceito** |
| [0013](0013-dynamic-routes-filter-sync-and-screen-gaps-resolution.md) | 2026-08-23 | Resolução de Gaps de Tela, Rotas Dinâmicas com SSG e Sincronização via URL | **Aceito** |
| [0012](0012-remove-firebase-tools-and-hosting.md) | 2026-08-23 | Remoção do firebase-tools e atualização de dependências vulneráveis | **Aceito** |
| [0011](0011-previews-and-branding-for-communities-events-companies.md) | 2026-08-19 | Visual Previews e Identidade de Marca para Ecossistema | **Aceito** |
| [0010](0010-project-visual-previews-and-showcase.md) | 2026-08-19 | Exibição de Visual Previews na Galeria e Vitrine de Projetos | **Aceito** |
| [0009](0009-corporate-modern-green-tech-design-system.md) | 2026-08-18 | Design System Green-Tech (Corporate Modern & Bio-Organic) | *Superado* |
| [0008](0008-migrate-to-nextjs-and-supabase.md) | 2026-08-17 | Migração para Next.js (App Router) e Supabase | **Aceito** |
| [0007](0007-rest-api-with-service-account-and-appcli.md) | 2026-08-15 | Automação e Deploy via REST API com Service Account | **Aceito** |
| [0006](0006-static-site-deploy.md) | 2026-08-13 | Deploy como site estático | **Aceito** |
| [0005](0005-simple-spa-with-hash-routing.md) | 2026-08-13 | SPA simples com hash routing | *Superado* |
| [0004](0004-stateless-auth-with-localstorage.md) | 2026-08-13 | Autenticação stateless simulada via localStorage | *Superado* |
| [0003](0003-design-system-css-variables.md) | 2026-08-13 | Design system próprio via CSS variables (Dark/Light) | *Superado* |
| [0002](0002-use-localstorage-as-database.md) | 2026-08-13 | Usar localStorage como banco de dados do MVP | *Superado* |
| [0001](0001-use-vanilla-html-css-js.md) | 2026-08-13 | Usar HTML/CSS/JS vanilla como stack inicial do MVP | *Superado* |

---

## Como usar este log

- Ao criar um novo ADR (`docs/adr/NNNN-titulo.md`), adicione a linha resumida
  no topo desta tabela **e** registre a entrada completa no
  [`README.md`](README.md), conforme o padrão do projeto.
