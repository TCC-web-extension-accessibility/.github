# ⚙️ Como configurar o ambiente

## 1. Crie uma pasta para o projeto

```bash
mkdir web-extension-accessibility/
```

---

## 2. Abra o VS Code como administrador

Abre a pasta criada no **VS Code** como **Administrador**. 

> 🔗 <u>**[Como abrir o VS Code como admin](https://github.com/TCC-web-extension-accessibility/.github/tree/main/OUTROS%20MATERIAIS%20-%20GERAL/ABRIR%20O%20VS%20CODE%20COMO%20ADMIN#abrir-o-vs-code-como-admin)**</u>

---

## 3. Clone os repositórios

```bash
cd web-extension-accessibility
git clone https://github.com/TCC-web-extension-accessibility/web-extension-accessibility-frontend.git
git clone https://github.com/TCC-web-extension-accessibility/web-extension-accessibility-backend.git
```

---

## 4. Configure seu Git global

```bash
git config --global user.name "Seu Nome"
git config --global user.email "seuemail@example.com"
```

---

## 5. Configure o remote (se necessário)

```bash
cd web-extension-accessibility-frontend
git remote -v

# Para alterar o remote (caso necessário)
git remote set-url origin https://github.com/TCC-web-extension-accessibility/web-extension-accessibility-frontend.git
```

Faça o mesmo para o repositório `web-extension-accessibility-backend`.

---

## 6. Instale as dependências

Para executar o projeto corretamente, é necessário instalar as dependências tanto do `frontend` quanto do `backend`. Acesse os links abaixo e siga as instruções conforme a estrutura do projeto:

- 📁 <u>**[Instruções do Frontend](https://github.com/TCC-web-extension-accessibility/web-extension-accessibility-frontend?tab=readme-ov-file#web-extension-accessibility-frontend)**</u>
- 📁 <u>**[Instruções do Backend](https://github.com/TCC-web-extension-accessibility/web-extension-accessibility-backend?tab=readme-ov-file#web-extension-accessibility-backend)**</u>

---

# 🚀 Trabalhando no projeto

Para os colaboradores internos da equipe que forem adicionar uma nova implementação ou quiserem alterar alguma funcionalidade, recurso ou estrutura do projeto, siga as etapas abaixo:

## 1. Criando uma nova branch a partir da `main`

Siga a estrutura:

- `feat/<código-task>-nome-da-feature` ➡ para nova funcionalidade ou recurso
- `fix/<código-task>-descricao-da-correcao` ➡ para correção de bug (erros específicos)
- Quer saber mais das outras convenções? Acesse <u>**[`Convenções das Branches`](https://github.com/TCC-web-extension-accessibility/.github/tree/main/OUTROS%20MATERIAIS%20-%20GERAL/CONVEN%C3%87%C3%95ES%20DAS%20BRANCHES#conven%C3%A7%C3%B5es-das-branches)**</u>

Execute os comandos no padrão abaixo:

```bash
git checkout main           # Garante que está na branch 'main'
git pull origin main        # Atualiza a 'main' local com o remoto
git checkout -b <tipo>/<código-task>-nome-da-feature
```

Substitua `nome-da-feature` por algo descritivo, como `initial-project-structure`.

> :information_source: <u>**[O que é o &lt;código-task&gt;?](https://github.com/TCC-web-extension-accessibility/.github/tree/main/OUTROS%20MATERIAIS%20-%20GERAL/O%20QUE%20%C3%89%20O%20C%C3%93DIGO-TASK#o-que-%C3%A9-o-c%C3%B3digo-task)**</u>

---

## 2. Trabalhando e commitando

- Faça as mudanças no código.
- Teste suas alterações localmente.
- E depois, adicione e commite as alterações.

```bash
git status          # Verifique os arquivos modificados
git add .           # Adicione todos os arquivos. TOME CUIDADO!!!
git commit -m "<tipo>/{RFxx}: descrição"
```

Acesse o link abaixo para saber mais sobre os padrões de commit do projeto:

> :blue_book: <u>**[Padrão de Commits](https://github.com/TCC-web-extension-accessibility/.github/tree/main/OUTROS%20MATERIAIS%20-%20GERAL/PADR%C3%83O%20DE%20COMMITS#padr%C3%A3o-de-commits)**</u>

---

## 3. Enviando para o GitHub

```bash
git push origin <tipo>/<código-task>-nome-da-feature
```

---

## **4. Abrindo um Pull Request (PR) para a `main`**

1. Vá até o repositório no GitHub
2. Clique em **"Compare & pull request"**
3. **Base branch**: `main`
4. **Compare branch**: `<tipo>/<código-task>-nome-da-feature`
5. Preencha o título e descrição
6. Clique em **"Create pull request"**

🎯 Esse PR será revisado e testado com outras features.

---

## **5. Testes e revisão na `main`**

- Todos os PRs (features, hotfixes, docs etc.) vão para `main`.
- Aqui verificamos se várias funcionalidades funcionam **juntas** sem conflito.

---


## **6. Atualize sua `main` e exclua branches**

Após o merge:

```bash
# Atualiza sua máquina
git checkout main
git pull origin main

# Exclui branch feature localmente e remotamente
git branch -d <tipo>/<código-task>-nome-da-feature               # local
git push origin --delete <tipo>/<código-task>-nome-da-feature    # remoto
```

Somente exclua as branches se não for mais usá-las! Para isso, acesse o link abaixo:

> :soap: <u>**[Por que excluir a branch &lt;tipo&gt;/* após o merge?](https://github.com/TCC-web-extension-accessibility/.github/tree/main/OUTROS%20MATERIAIS%20-%20GERAL/PORQUE%20EXCLUIR%20A%20BRANCH%20DE%20DESENVOLVIMENTO%20AP%C3%93S%20O%20MERGE#por-que-excluir-a-branch-tipo-ap%C3%B3s-o-merge)**</u>

---

## 💡 Exemplo completo

```bash
# Criar nova funcionalidade
git checkout main
git pull origin main
git checkout -b <tipo>/<código-task>-nome-da-feature
# codifica...
git add .
git commit -m "<tipo>/{RFxx}: <descrição>"
git push origin <tipo>/<código-task>-nome-da-feature

# ETAPA 4 - GitHub: PR da '<tipo>/<código-task>-nome-da-feature' → 'main'

# Depois que várias features forem testadas (ETAPA 5), faça a ETAPA 6!
```
