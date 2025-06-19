# INSTALAR O PYTHON E PIP (MÚLTIPLAS VERSÕES)

## ⏩ PASSO 1 - Instalar o Python (caso ainda não tenha)

1. Vá até o site oficial: https://www.python.org/downloads/windows/
2. Baixe a versão recomendada para Windows (por ex. Python 3.12.3).
3. Durante a instalação:
    - Clique em **Customize installation**
    - Marque **pip**
    - Marque **Add Python to environment variables**
    - Na próxima tela, altere o caminho de instalação para:
        
        ```
        C:\Users\SeuNome\AppData\Local\Programs\Python\Pythonxxx
        ```
        
    - Depois clique em **"Install Now"**
    
    > 📍 Isso instala o **Python e o pip junto automaticamente**.
    

---

## ✅ PASSO 2 - Verifique se o pip está funcionando para as duas versões

Abra o `cmd` e teste:

**Exemplo (Python 3.8):**

```bash
C:\Users\SeuNome\AppData\Local\Programs\Python\Python38\python.exe -m pip --version
```

**Exemplo (Python 3.12.3):**

```bash
C:\Users\SeuNome\AppData\Local\Programs\Python\Python312\python.exe -m pip --version
```

Se ambos mostrarem versões válidas do `pip`, está tudo certo!

---

## ✅ PASSO 3 - Adicione apelidos para facilitar no terminal

Você pode **criar aliases** no terminal para usar algo como:

```bash
py38 -m pip install numpy
py312 -m pip install pandas
```

### Como fazer:

1. Crie um arquivo chamado `aliases.bat` em **"C:\Users\SeuNome\”** com o seguinte conteúdo:

```
@echo off
doskey py38="C:\Users\SeuNome\AppData\Local\Programs\Python\Python38\python.exe" $*
doskey py312="C:\Users\SeuNome\AppData\Local\Programs\Python\Python312\python.exe" $*
```

2. Toda vez que for abrir o terminal, digite:

```bash
call "C:\Users\SeuNome\aliases.bat"
```

Ou adicione isso ao atalho de inicialização do cmd.

---

## ✅ **Passo 3.1 – Criar um atalho para o terminal que execute o script**

1. Vá até a **Área de Trabalho**
2. Clique com o botão direito > **Novo > Atalho**
3. Na caixa “Digite a localização do item”, coloque:

```
cmd /k "C:\Users\SeuNome\aliases.bat"
```

1. Clique em **Avançar**, e nomeie como:

```
Terminal Python
```

2. Clique em **Concluir**

---

## ✅ **Passo 3.2 – Usar os atalhos**

Agora, sempre que quiser trabalhar com Python, **abra o atalho "Terminal Python"** que você criou.

Você poderá usar:

```bash
py38 --version
py38 -m pip list

py312 --version
py312 -m pip list
```

---

## ✅ **Passo 4** Verificar se seu ambiente está 100% configurado:

```bash
where python
where pip
python --version
pip --version
```

Assim vamos ver exatamente onde estão os caminhos e se está tudo certo.

### ✅ **Passo 4.1** **Estrutura Final Esperada**

```
C:\Users\SeuNome>where python
C:\Users\SeuNome\AppData\Local\Programs\Python\Python312\python.exe
C:\Program Files\MySQL\MySQL Shell 8.4\bin\python.exe
C:\Users\SeuNome\AppData\Local\Programs\Python\Python38\python.exe
C:\Users\SeuNome\AppData\Local\Microsoft\WindowsApps\python.exe

C:\Users\SeuNome>where pip
C:\Users\SeuNome\pip
C:\Users\SeuNome\AppData\Local\Programs\Python\Python38\Scripts\pip.exe
C:\Users\SeuNome\AppData\Roaming\Python\Python312\Scripts\pip.exe

C:\Users\SeuNome>python --version
Python 3.12.3

C:\Users\SeuNome>pip --version
pip 24.0 from C:\Users\SeuNome\AppData\Local\Programs\Python\Python312\lib\site-packages\pip (python 3.12)
```