# 👨‍💻 [TCC - Web Extension Accessibility](https://github.com/TCC-web-extension-accessibility)

Repositório da organização do projeto [**Web Extension Accessibility**](https://github.com/TCC-web-extension-accessibility), desenvolvido como parte de um Trabalho de Conclusão de Curso. Este projeto tem como objetivo principal **criar uma pacote de acessibilidade web**, visando proporcionar **melhor experiência de navegação nos sites de internet para pessoas com deficiência**.

## 🧩 Estrutura da Organização

Este projeto está dividido nos seguintes repositórios:

- [`.github`](https://github.com/TCC-web-extension-accessibility/.github) - Documentação e configurações da organização.
- [`web-extension-accessibility-frontend`](https://github.com/TCC-web-extension-accessibility/web-extension-accessibility-frontend) - Interface gráfica, componentes visuais e interação com o usuário.
- [`web-extension-accessibility-backend`](https://github.com/TCC-web-extension-accessibility/web-extension-accessibility-backend) - APIs, lógica de negócio, banco de dados e integrações com IA.

---

## 📝 Requisitos Funcionais
  
Acesse o link abaixo para saber os requisitos funcionais do sistema:

<div>
<a 
  href="https://github.com/TCC-web-extension-accessibility/.github/tree/main/OUTROS%20MATERIAIS%20-%20GERAL/REQUISITOS%20FUNCIONAIS#requisitos-funcionais" 
  target="_blank"
  style="  
    display: block;     
    background-color: #3a2c1f; 
    color: #FFFAFA; 
    text-decoration: none; 
    padding: 15px 30px; 
    border-radius: 8px;
    font-weight: 600;">
  📝 <u>Requisitos Funcionais</u>
</a>
</div>

## 📝 Requisitos Não Funcionais

Acesse o link abaixo para saber os requisitos não funcionais do sistema:

<div>
<a 
  href="https://github.com/TCC-web-extension-accessibility/.github/tree/main/OUTROS%20MATERIAIS%20-%20GERAL/REQUISITOS%20N%C3%83O%20FUNCIONAIS#requisitos-n%C3%A3o-funcionais" 
  target="_blank"
  style="  
    display: block;     
    background-color: #3a2c1f; 
    color: #FFFAFA; 
    text-decoration: none; 
    padding: 15px 30px; 
    border-radius: 8px;
    font-weight: 600;">
  📝 <u>Requisitos Não Funcionais</u>
</a>
</div>

---

# 1. Crie uma pasta em seu computador

Esta pasta serve para armazenar o projeto

```bash
mkdir web-extension-accessibility/
```

---

# 2. Execute **SEMPRE** o **VS Code** como Administrador

Abre a pasta criada no **VS Code** como **Administrador**. 

> Acesse o link abaixo para saber como deixar o **VS Code** como Administrador.

<div>
<a 
  href="https://github.com/TCC-web-extension-accessibility/.github/tree/main/OUTROS%20MATERIAIS%20-%20GERAL/ABRIR%20O%20VS%20CODE%20COMO%20ADMIN#abrir-o-vs-code-como-admin" 
  target="_blank"
  style="  
    display: block;     
    background-color: #131e3d; 
    color: #FFFAFA; 
    text-decoration: none; 
    padding: 15px 30px; 
    border-radius: 8px;
    font-weight: 600;">
  💻 <u>ABRIR O VS CODE COMO ADMIN</u>
</a>
</div>

---

# 🚀 Como baixar e utilizar o projeto

## 1. Clone os repositórios

### Acesse a pasta `web-extension-accessibility/` e clone os repositórios

Antes de clonar os projetos, acesse a pasta criada para armazenar os repositórios:

```bash
cd web-extension-accessibility
```

### Clone do repositório frontend

```bash
git clone https://github.com/TCC-web-extension-accessibility/web-extension-accessibility-frontend.git
```

### Clone do repositório backend

```bash
git clone https://github.com/TCC-web-extension-accessibility/web-extension-accessibility-backend.git
```

---

## 2. Configure seu Git global

```bash
git config --global user.name "Seu Nome"
git config --global user.email "seuemail@example.com"
```

---

## 3. Acesse a pasta e configure o remote (se necessário)

```bash
cd web-extension-accessibility-frontend
git remote -v

# Para alterar o remote (caso necessário)
git remote set-url origin https://github.com/TCC-web-extension-accessibility/web-extension-accessibility-frontend.git
```

Faça o mesmo para o repositório `web-extension-accessibility-backend`.

---

## 4. Instalar as dependências do projeto

Para executar o projeto corretamente, é necessário instalar as dependências tanto do frontend quanto do backend. Siga as instruções abaixo conforme a estrutura do projeto.

### 4.1 Frontend (`web-extension-accessibility-frontend/`)

Para configurar e executar o projeto de `frontend`, acesse as instruções no link abaixo 👇

<div>
<a 
  href="https://github.com/TCC-web-extension-accessibility/web-extension-accessibility-frontend?tab=readme-ov-file#web-extension-accessibility-frontend" 
  target="_blank"
  style="  
    display: block;     
    background-color: #4a1212; 
    color: #FFFAFA; 
    text-decoration: none; 
    padding: 15px 30px; 
    border-radius: 8px;
    font-weight: 600;">
  📁 <u>CONFIGURAR E EXECUTAR - Web Extension Accessibility Frontend</u>
</a>
</div>

---

### 4.2 Backend (`web-extension-accessibility-backend/`)

Para configurar e executar o projeto de `backend`, acesse as instruções no link abaixo 👇

<div>
<a 
  href="https://github.com/TCC-web-extension-accessibility/web-extension-accessibility-backend?tab=readme-ov-file#web-extension-accessibility-backend" 
  target="_blank"
  style="  
    display: block;     
    background-color: #4a1212; 
    color: #FFFAFA; 
    text-decoration: none; 
    padding: 15px 30px; 
    border-radius: 8px;
    font-weight: 600;">
  📁 <u>CONFIGURAR E EXECUTAR - Web Extension Accessibility Backend</u>
</a>
</div>

---

## 5. Crie uma nova branch a partir da `main`

Siga a estrutura:

- `feat/<código-task>-nome-da-feature`
- `fix/<código-task>-descricao-da-correcao`
- Quer saber mais das outras convenções? Acesse [`Convenções das Branches`]()

Execute os comandos no padrão abaixo:

```bash
git checkout main           # Garante que está na branch main
git pull origin main        # Atualiza a main local com o remoto
git checkout -b <tipo>/<código-task>-nome-da-feature
```

Substitua `nome-da-feature` por algo descritivo, como `initial-project-structure`.

<div>
<a 
  href="https://github.com/TCC-web-extension-accessibility/.github/tree/main/OUTROS%20MATERIAIS%20-%20GERAL/O%20QUE%20%C3%89%20O%20C%C3%93DIGO-TASK#o-que-%C3%A9-o-c%C3%B3digo-task" 
  target="_blank"
  style="  
    display: block;     
    background-color: #251538; 
    color: #FFFAFA; 
    text-decoration: none; 
    padding: 15px 30px; 
    border-radius: 8px;
    font-weight: 600;">
  ❓ <u>O que é o &lt;código-task&gt;?</u>
</a>
</div>


---

## 6. Trabalhe, adicione e commite suas alterações

- Faça as mudanças no código.
- Teste suas alterações localmente.
- E depois, adicione e commite as alterações.

```bash
# Verifique os arquivos modificados
git status

# Adicione os arquivos
git add .   # Adiciona todos! TOME CUIDADO!!!

# Faça o commit
git commit -m "Siga o padrão de commits do projeto que está no link abaixo 👇"
```

Acesse o link abaixo para saber mais sobre os padrões de commit do projeto:

<div>
<a 
  href="https://github.com/TCC-web-extension-accessibility/.github/tree/main/OUTROS%20MATERIAIS%20-%20GERAL/PADR%C3%83O%20DE%20COMMITS#padr%C3%A3o-de-commits" 
  target="_blank"
  style="  
    display: block;     
    background-color: #3a2c1f; 
    color: #FFFAFA; 
    text-decoration: none; 
    padding: 15px 30px; 
    border-radius: 8px;
    font-weight: 600;">
  📘 <u>Padrão de Commits</u>
</a>
</div>

---

## 7. Envie sua branch para o GitHub

```bash
git push origin <tipo>/<código-task>-nome-da-feature
```

---

## **8. Abrir Pull Request (PR) para `main`**

No GitHub:

- Vá até o repositório.
- Clique em **"Compare & pull request"**.
- **Base branch**: `main`
- **Compare branch**: `<tipo>/<código-task>-nome-da-feature`
- Preencha o título e descrição
- Clique em **"Create pull request"**.

🎯 Esse PR será revisado e testado com outras features.

---

## **9. Testes e revisão na branch `main`**

- Todos os PRs (features, hotfixes, docs etc.) vão para `main`.
- Aqui verificamos se várias funcionalidades funcionam **juntas** sem conflito.

---


## **10. Atualizar `main` e excluir branches**

Após o merge:

```bash
# Atualiza sua máquina
git checkout main
git pull origin main

# Exclui branch feature localmente e remotamente
git branch -d <tipo>/<código-task>-nome-da-feature               # local
git push origin --delete <tipo>/<código-task>-nome-da-feature    # remoto
```

Somente exclua as branches se não for mais usá-las 👇

<div>
<a 
  href="https://github.com/TCC-web-extension-accessibility/.github/tree/main/OUTROS%20MATERIAIS%20-%20GERAL/PORQUE%20EXCLUIR%20A%20BRANCH%20DE%20DESENVOLVIMENTO%20AP%C3%93S%20O%20MERGE#por-que-excluir-a-branch-tipo-ap%C3%B3s-o-merge" 
  target="_blank"
  style="  
    display: block;     
    background-color: #251538; 
    color: #FFFAFA; 
    text-decoration: none; 
    padding: 15px 30px; 
    border-radius: 8px;
    font-weight: 600;">
  🧹 <u>Por que excluir a branch &lt;tipo&gt;/* após o merge?</u>
</a>
</div>

---

## 🔐 Exemplo real

---
```bash
# Criar nova funcionalidade
git checkout main
git pull origin main
git checkout -b <tipo>/<código-task>-nome-da-feature
# codifica...
git add .
git commit -m "<tipo>/{RFxx}: <descrição>"
git push origin <tipo>/<código-task>-nome-da-feature

# ETAPA 8 - GitHub: PR da '<tipo>/<código-task>-nome-da-feature' → 'main'

# Depois que várias features forem testadas, faça a ETAPA 10
```