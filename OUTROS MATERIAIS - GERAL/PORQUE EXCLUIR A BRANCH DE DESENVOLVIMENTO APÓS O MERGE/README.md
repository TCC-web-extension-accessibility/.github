# Por que Excluir a Branch &lt;tipo&gt;/* após o Merge?

### ✅ 1. **Evita bagunça no repositório**

- Sem limpeza, o repositório fica cheio de branches antigas e inúteis.
- Branches que já foram *mergeadas* não têm mais função.

---

### ✅ 2. **Indica que aquela feature já está entregue**

- A exclusão sinaliza que a tarefa foi **finalizada e entregue** na `main`.

---

### ✅ 3. **Facilita manutenção**

- Menos branches = menos confusão.
- Evita alguém sem querer continuar codando em uma branch já finalizada.

---

### ✅ 4. **Evita conflitos futuros**

- Se você continuar trabalhando em uma branch antiga depois de várias mudanças na `main`, pode gerar **conflitos difíceis de resolver**.

---

## ⚠️ E se eu quiser manter por backup?

Não precisa! O histórico da branch e todos os commits **ainda ficam disponíveis** no Git mesmo depois que a branch é excluída, já que os commits foram incorporados no merge.

Você pode recuperar a branch facilmente, se necessário:

```bash
git checkout -b <tipo>/<código-task>-nome-da-feature <commit_hash>
```

---

## 💻 Como excluir a branch

### 🔨 Localmente:

```bash
git branch -d <tipo>/<código-task>-nome-da-feature 
# -d só permite excluir se já foi mergeada
```

### 🌐 No GitHub (remoto):

```bash
git push origin --delete <tipo>/<código-task>-nome-da-feature
```

---

## 📌 Conclusão

| Situação após o merge da feature | Devo excluir a branch? |
| --- | --- |
| PR da `<tipo>/*` foi mergeado na `main` | ✅ Sim |
| PR ainda está aberto ou em revisão | ❌ Não |
| Branch será reutilizada para a mesma tarefa (não finalizada) | ❌ Não |