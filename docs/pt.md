# Minhas configurações do meu Windows Terminal no Windows 11

![image](https://github.com/josuenm/my-windows-terminal/assets/83486074/c41fe415-cbcf-4f69-a612-ad5610e13147)
![image](https://github.com/josuenm/my-windows-terminal/assets/83486074/53e69201-42a1-4237-85a9-c7fe3ef63ac7)

## Instruções

1. clique <a href="https://apps.microsoft.com/store/detail/windows-terminal/9N0DX20HK701?hl=pt-br&gl=br&icid=CNavAppsWindowsApps" target="_blank">aqui</a> para baixar o windows terminal na loja da microsoft
2. clique <a href="https://apps.microsoft.com/store/detail/powershell/9MZ1SNWT0N5D" target="_blank">aqui</a> para baixar o powershell na loja da microsoft
3. abra seu windows terminal e coloque o powershell como padrão

### Instalar pacotes

1. abra seu windows terminal e instale o scoop com o comando `iwr -useb get.scoop.sh | iex`
2. instale o jq com o commando `scoop install curl sudo jq`
3. instale o neovim com o comando `scoop install neovim gcc`
4. instale o posh-git com o comando `Install-Module posh-git -Scope CurrentUser -Force`
5. instale o Terminal-Icons com o comando `Install-Module Terminal-Icons -Scope CurrentUser -Force`
6. instale oh-my-posh com o comando `scoop install https://github.com/JanDeDobbeleer/oh-my-posh/releases/latest/download/oh-my-posh.json`, but if you can't install just click <a href="ms-windows-store://pdp/?productid=XP8K0HKJFRXGCK" target="_blank">here</a>

### Como customizar o Windows Terminal

1. configure a aparência para usar o modo transparente e use sua cor favorita
2. copie os arquivos "josuenm-omp.json" e "user_profile.ps1"
3. entre em "C:/Users/seu-usuário/.config/" e crie a pasta "powershell" e cole os arquivos la dentro
4. agora abra o seu windows terminal e digite `nvim $PROFILE.CurrentUserCurrentHost` e pressione `ctrl C` e digite `:wq` para salvar e sair do neovim
5. digite "a" para editar o arquivo, cole esse código `. $env:USERPROFILE\.config\powershell\user_profile.ps1`
