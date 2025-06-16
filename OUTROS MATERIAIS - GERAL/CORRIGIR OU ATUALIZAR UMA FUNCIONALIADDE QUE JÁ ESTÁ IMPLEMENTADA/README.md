# Corrigir ou Atualizar uma Funcionalidade que já está Implementada

## Atualizações em Funcionalidades Existentes

Caso seja necessário realizar **ajustes, correções ou melhorias** em funcionalidades já implementadas, utilizamos os seguintes padrões de branch:

- `fix/<código-task>-nome-da-feature` – para correções de bugs
- `improvement/<código-task>-nome-da-feature` ou `enhancement/<código-task>-nome-da-feature` – para melhorias não relacionadas a bugs
- `refactor/<código-task>-nome-da-feature` – para mudanças estruturais internas no código

---

### ✅ Para **correção** de uma funcionalidade já implementada (bug fix):

**Branch**:

`fix/<código-task>-nome-da-feature`

📌 Use quando for corrigir um erro relacionado a uma funcionalidade específica já em uso.

**Exemplo**:

`fix/<código-task>-login-authentication` → Corrigindo problema na autenticação do login

---

### ✅ Para **atualização ou melhoria** de uma funcionalidade (sem bug):

**Branch**:

`improvement/<código-task>-nome-da-feature` ou `enhancement/<código-task>-nome-da-feature`

📌 Use para melhorias de performance, UX, código ou comportamento da funcionalidade.

**Exemplo**:

`improvement/<código-task>-user-profile-loading` → Otimizando carregamento do perfil do usuário

---

### ✅ Para **refatoração interna** da funcionalidade (sem mudar comportamento):

**Branch**:

`refactor/<código-task>-nome-da-feature`

📌 Use se estiver reorganizando código, renomeando variáveis, simplificando lógica, mas sem alterar a lógica final.

**Exemplo**:

`refactor/<código-task>-payment-methods` → Refatorando estrutura do módulo de pagamentos