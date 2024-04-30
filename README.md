# Instalación de Zsh + Oh My Zsh + plugins

Este documento detalla los pasos para instalar Zsh, Oh My Zsh y algunos plugins útiles en tu sistema.

## Pasos

1. **Actualizar el sistema:**
   ```bash
   sudo apt update
   sudo apt upgrade

2. **Descargar Zsh:**
    ```bash
    sudo apt install zsh

3. **Descargar Oh My Zsh:**
    ```bash
    sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"

4. **Descargar tema powerlevel10k:**
    ```bash
    git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k

5. **Modificar el tema:**
    ```bash
    nano .zshrc
    ZSH_THEME="powerlevel10k/powerlevel10k"

6. **Iniciar el asistente:**
    ```bash
    source ~/.zshrc

7. **Instalar plugins:**
    ```bash
    git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
    
    git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting

8. **Activar plugins:**
    ```bash
    nano .zshrc

    plugins=(git
        zsh-syntax-highlighting
        zsh-autosuggestions
    )

    source ~/.zshrc

9. **Cambiar la apariencia:**
    ```bash
    Cambiar la apariencia de windows terminal a Campbell

10. **Instalar Docker:**
    ```bash
    YT:		https://www.youtube.com/watch?v=A34k_dp8CxM
    Doc:	https://docs.docker.com/engine/install/ubuntu/