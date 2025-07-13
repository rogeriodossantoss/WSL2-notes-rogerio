🧼 1. Remover a instalação corrompida
No PowerShell ou CMD (como administrador), execute:

wsl --unregister Ubuntu-22.04

Esse comando remove completamente a distribuição quebrada do WSL.

💾 Passo 2: Reinstalar o Ubuntu 22.04
Execute no terminal:

wsl --install -d Ubuntu-22.04

⚙️ 3. Verifique se está usando WSL 2
Se quiser garantir que o WSL 2 está habilitado corretamente:

wsl --set-default-version 2

🔒 Dica: Fazer backup da distribuição
Depois de reinstalar e configurar, você pode exportar para um backup seguro:

wsl --export Ubuntu-22.04 ubuntu_backup.tar
E restaurar no futuro com:

wsl --import Ubuntu-22.04-restaurada C:\WSL\UbuntuRestaurada ubuntu_backup.tar
