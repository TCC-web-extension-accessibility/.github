# Abrir o VS CODE como ADMIN

Para criar um **atalho do Visual Studio Code (VS Code) que sempre abre como administrador** em **Windows, Linux e macOS**, siga os passos específicos para cada sistema operacional:

---

### 💻 **Windows**

No Windows, você pode criar um atalho que abre o VS Code como administrador com os seguintes passos:

### ✅ Passos:

1. **Crie um atalho do VS Code:**
    - Vá até `C:\Users\SeuUsuario\AppData\Local\Programs\Microsoft VS Code\Code.exe`.
    - Clique com o botão direito em `Code.exe` > **Enviar para > Área de trabalho (criar atalho)**.
2. **Configure o atalho para abrir como administrador:**
    - Clique com o botão direito no atalho na área de trabalho > **Propriedades**.
    - Vá na aba **Atalho** > clique em **Avançado...**.
    - Marque a opção **Executar como administrador**.
    - Clique em **OK** > **Aplicar** > **OK**.

### 🔁 Observação:

- O Windows sempre solicitará permissão via UAC ao abrir como administrador.

---

### 🐧 **Linux**

No Linux, o conceito de “executar como administrador” geralmente se refere a abrir o VS Code com `sudo`, mas por padrão, **softwares gráficos não devem ser abertos com `sudo` diretamente**, pois isso pode gerar problemas com permissões.

### ✅ Alternativas seguras:

1. **Crie um atalho com `pkexec` (polkit):**
    1. Crie um script chamado `code-admin.sh`:
        
        ```bash
        #!/bin/bash
        pkexec env DISPLAY=$DISPLAY XAUTHORITY=$XAUTHORITY code
        ```
        
    2. Torne o script executável:
        
        ```bash
        chmod +x ~/code-admin.sh
        ```
        
    3. Crie um atalho `.desktop` com esse script:
        
        ```bash
        nano ~/.local/share/applications/code-admin.desktop
        ```
        
        Conteúdo:
        
        ```
        [Desktop Entry]
        Name=VS Code (Admin)
        Exec=/home/seu_usuario/code-admin.sh
        Icon=code
        Type=Application
        Terminal=false
        Categories=Development;
        ```
        
    4. Atualize os atalhos:
        
        ```bash
        update-desktop-database ~/.local/share/applications
        ```
        
2. **Use o terminal apenas para abrir como root (menos recomendado):**
    
    ```bash
    sudo code
    ```
    

---

### 🍎 **macOS**

No macOS, abrir o VS Code como "administrador" requer o uso do terminal com `sudo`, mas **apps GUI não devem ser abertos diretamente com `sudo`**, pois o sistema é mais restritivo.

### ✅ Solução alternativa:

1. **Crie um AppleScript para solicitar permissão de administrador:**
    - Abra o app **Script Editor** e cole:
        
        ```
        do shell script "open -a 'Visual Studio Code'" with administrator privileges
        ```
        
    - Salve como **Aplicativo** com o nome `VS Code Admin.app`.
2. **Coloque o aplicativo no Dock ou crie atalho no Finder.**

### ⚠️ Observação:

- O macOS solicitará a senha de administrador sempre que abrir esse app.

---

### ✅ Conclusão

| Sistema | Solução recomendada |
| --- | --- |
| Windows | Criar atalho e marcar “Executar como administrador” |
| Linux | Usar `pkexec` via script + `.desktop` |
| macOS | Criar AppleScript como aplicativo que abre o VS Code com privilégios elevados |