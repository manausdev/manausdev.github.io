# ADR 0027: Auditoria de acessibilidade, performance e CI

- **Data:** 2026-10-20
- **Status:** Aceito
- **Domínio:** Qualidade / DevOps / Acessibilidade

## Contexto

As automações identificaram oportunidades acionáveis na aplicação e no fluxo de
integração:

- alguns formulários tinham rótulos sem vínculo explícito com seus controles;
- a homepage executava consultas `head` duplicadas para obter contagens que já
  podiam ser reaproveitadas das consultas de listagem;
- a CI não declarava permissões mínimas nem cancelava execuções obsoletas da
  mesma referência;
- não havia issues abertas ou telemetria existente que justificassem uma
  alteração adicional de produto.

## Decisão

Adotar as seguintes correções de baixo risco:

1. Associar cada `label` aos respectivos `input`, `select` e `textarea` por
   `htmlFor`/`id`, preservando o comportamento dos formulários e melhorando a
   navegação por leitor de tela.
2. Reutilizar os campos `count` das consultas de projetos e vagas na homepage,
   removendo duas requisições `head` redundantes e mantendo o fallback para o
   tamanho da lista retornada.
3. Declarar `contents: read` na workflow da CI e usar `concurrency` com
   `cancel-in-progress` para evitar execuções obsoletas consumindo recursos.
4. Não adicionar analytics ou telemetria invasiva sem uma necessidade de produto,
   consentimento e decisão de privacidade explícitos.

## Consequências

- Formulários ficam mais acessíveis sem alterar sua API ou validação.
- A homepage reduz round-trips ao Supabase em produção.
- Pull requests e pushes recebem feedback mais rápido quando há novas execuções.
- A ausência de telemetria permanece uma decisão consciente, a ser revisitada
  somente com requisitos claros de produto e privacidade.

## Validação

Foi executado `git diff --check`, `npm test`, `npm run typecheck` e `npm run build`
com Node.js 24 instalado via NVM.
