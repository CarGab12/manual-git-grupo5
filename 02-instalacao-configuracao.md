Instalação e Configuração do Git
Onde baixar e instalar o Git
🪟 Windows
Acesse: https://git-scm.com/download/win

Baixe o instalador.

Execute e siga as etapas padrão (pode deixar as opções marcadas como estão).

Após a instalação, o terminal Git Bash estará disponível.

🍎 macOS
Instale via Homebrew:

brew install git
Ou baixe diretamente em: https://git-scm.com/download/mac

🐧 Linux (Debian/Ubuntu)
Abra o terminal e digite:

sudo apt update
sudo apt install git
Configuração Inicial do Git
Após instalar o Git, você deve configurar seu nome e e-mail. Isso é importante porque cada commit que você fizer será identificado com essas informações.

Comandos de configuração:
git config --global user.name "Seu Nome"
git config --global user.email "seu@email.com"
Esses dados aparecerão nos commits como:


Author: Seu Nome <seu@email.com>
Verificando a configuração atual
git config --list
Isso mostrará todas as configurações atuais do Git no seu sistema.

Checando se o Git está instalado corretamente
Execute:


git --version
Você verá algo como:

git version 2.44.0
Isso confirma que a instalação foi concluída com sucesso.

✅ Agora o Git está instalado e configurado, pronto para ser usado!
