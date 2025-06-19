# Convenções das Branches

A estrutura de branches utilizada segue uma abordagem que separa o ambiente de produção, o ambiente de desenvolvimento e as funcionalidades em progresso, conforme descrito a seguir:

- **`main`:** branch principal, destinada a conter o código estável e pronto para produção.
- **`<tipo>/<código-task>-nome-da-tarefa`:** branches específicas para o desenvolvimento de cada funcionalidade, ajuste, correção, refatoração ou atualização, a serem integradas posteriormente na branch `main`.

> ❓ <u>**[O que é o &lt;código-task&gt;?](https://github.com/TCC-web-extension-accessibility/.github/tree/main/OUTROS%20MATERIAIS%20-%20GERAL/O%20QUE%20%C3%89%20O%20C%C3%93DIGO-TASK#o-que-%C3%A9-o-c%C3%B3digo-task)**</u>

---

## Convenções para Branches de desenvolvimento

| Tipo de Alteração | Nome da Branch | Observações |
| --- | --- | --- |
| Recurso/Funcionalidade nova | `feat/<código-task>-nome-da-feature` | Ligada a um RF (Requisito Funcional)provavelmente |
| Correção de bug | `fix/<código-task>-descricao-do-bug` | Para resolver erros específicos |
| Ajuste ou melhoria na arquitetura | `chore/<código-task>-estrutura`, `chore/<código-task>-arquitetura` | Por exemplo: reestruturação de pastas, modularização |
| Refatoração de código | `refactor/<código-task>-nome-do-modulo` | Para mudanças que melhoram o código sem alterar funcionalidades |
| Atualização de dependência, script, etc | `chore/<código-task>-dependencias`, `chore/<código-task>-scripts` | Mudanças não relacionadas diretamente a código de negócio |
| Alteração em arquivos de documentação	| `docs/<código-task>-descricao-da-alteracao` |	Mudança no `README.md`, ou, em outros arquivos de documentação que não envolvem código funcional do sistema

---

✅ <u>**[Corrigir ou Atualizar uma Funcionalidade que já está Implementada](https://github.com/TCC-web-extension-accessibility/.github/tree/main/OUTROS%20MATERIAIS%20-%20GERAL/CORRIGIR%20OU%20ATUALIZAR%20UMA%20FUNCIONALIADDE%20QUE%20J%C3%81%20EST%C3%81%20IMPLEMENTADA)**</u>
