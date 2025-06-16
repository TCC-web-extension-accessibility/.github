# Padrão de Commits

Para complementar as práticas acima, nesse tópico serão especificados os formatos e convenções para as mensagens de commit, garantindo clareza e rastreabilidade no histórico de alterações. A seguir, vemos as diretrizes adotadas:

---

Cada commit deve seguir os formatos:

- Com Requisito Funcional:
    ```
    <tipo>/{RFxx}: <descrição> 
    ```

- Sem Requisito Funcional:
    ```
    <tipo>: <descrição> 
    ```

---

### 🧩 **Tipos de Commit (&lt;tipo&gt;) -** https://github.com/iuricode/padroes-de-commits

| &lt;tipo&gt; | Quando usar |
| --- | --- |
| `feat:` | Commits do tipo feat indicam que seu trecho de código está incluindo um novo recurso/funcionalidade (se relaciona com o MINOR do versionamento semântico). |
| `fix:` | Commits do tipo fix indicam que seu trecho de código commitado está solucionando um problema (bug fix), (se relaciona com o PATCH do versionamento semântico). Para **correção de bugs** (inclusive relacionados a funcionalidades RF). |
| `docs:` | Commits do tipo docs indicam que houveram mudanças na documentação, como por exemplo no Readme do seu repositório, comentários, etc. (Não inclui alterações em código). |
| `test:` | Commits do tipo test são utilizados quando são realizadas alterações em testes, seja criando, alterando ou excluindo testes unitários. (Não inclui alterações em código). |
| `build:` | Commits do tipo build são utilizados quando são realizadas modificações em arquivos de build e dependências. |
| `perf:` | Commits do tipo perf servem para identificar quaisquer alterações de código que estejam relacionadas a performance. |
| `style:` | Para alterações **visuais** (HTML/CSS, layout) **sem alterar lógica de código.** |
| `refactor:` `improvement:` `enhancement:` | Commits do tipo refactor referem-se a mudanças devido a refatorações que não alterem sua funcionalidade, como por exemplo, uma alteração no formato como é processada determinada parte da tela, mas que manteve a mesma funcionalidade, ou melhorias de performance devido a um code review. |
| `chore:` | Commits do tipo chore indicam atualizações de tarefas de build, configurações de administrador, pacotes... como por exemplo adicionar um pacote no gitignore. (Não inclui alterações em código). |
| `ci:` | Commits do tipo ci indicam mudanças relacionadas a integração contínua (continuous integration). |
| `raw:` | Commits do tipo raw indicam mudanças relacionadas a arquivos de configurações, dados, features, parâmetros. |
| `cleanup:` | Commits do tipo cleanup são utilizados para remover código comentado, trechos desnecessários ou qualquer outra forma de limpeza do código-fonte, visando aprimorar sua legibilidade e manutenibilidade. |
| `remove:` | Commits do tipo remove indicam a exclusão de arquivos, diretórios ou funcionalidades obsoletas ou não utilizadas, reduzindo o tamanho e a complexidade do projeto e mantendo-o mais organizado. |

---

### 📝 **Exemplos de Commits**

### ✔ Com RF (funcionalidade):

```
feat/{RF02}: implementar botão de aumentar e diminuir fonte
```

```
fix/{RF05}: corrigir aplicação do modo alto contraste
```

```
style/{RF02}: modificar a estilização do botão de aumentar e diminuir fonte
```

### 🚫 Sem RF (infraestrutura ou suporte):

```
style: implementar a interface inicial do menu de acessibilidade
```

```
chore: adicionar eslint e prettier para padronização de código
```

```
docs: adicionar instruções de instalação no README
```

---

### ⚠️ **Regras Gerais**

- Sempre comece com **“&lt;tipo&gt;/”** seguido do código do requisito funcional (RF01, RF02 etc.). Se não for relacionado a uma funcionalidade, não coloque nada.
  - Exemplo de commit com Requisito Funcional: `<tipo>/{RFxx}: <descrição>`.
  - Exemplo de commit sem Requisito Funcional: `<tipo>: <descrição>`.
- Mantenha a **descrição concisa e no imperativo** (ex: “implementar”, “corrigir”, “ajustar”).
  