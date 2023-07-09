# My Windows 11 terminal configuration

![image](https://github.com/josuenm/my-windows-terminal/assets/83486074/c41fe415-cbcf-4f69-a612-ad5610e13147)
![image](https://github.com/josuenm/my-windows-terminal/assets/83486074/53e69201-42a1-4237-85a9-c7fe3ef63ac7)

## Instructions

1. click <a href="https://apps.microsoft.com/store/detail/windows-terminal/9N0DX20HK701?hl=pt-br&gl=br&icid=CNavAppsWindowsApps" target="_blank">here</a> to download windows terminal on microsoft store
2. click <a href="https://apps.microsoft.com/store/detail/powershell/9MZ1SNWT0N5D" target="_blank">here</a> to download powershell
3. go to your windows terminal and set powershell as default

### Install packages

1. open your windows terminal and isntall scoop with command `iwr -useb get.scoop.sh | iex`
2. install jq with command `scoop install curl sudo jq`
3. isntall neovim with command `scoop install neovim gcc`
4. install posh-git with command `Install-Module posh-git -Scope CurrentUser -Force`
5. install Terminal-Icons with command `Install-Module Terminal-Icons -Scope CurrentUser -Force`
6. install oh-my-posh with command `scoop install https://github.com/JanDeDobbeleer/oh-my-posh/releases/latest/download/oh-my-posh.json`, but if you can't install just click <a href="ms-windows-store://pdp/?productid=XP8K0HKJFRXGCK" target="_blank">here</a>

### How custom windows terminal

1. configure the appareance to use transparent mode and set to your best color
2. copy "josuenm-omp.json" and "user_profile.ps1"
3. go to "C:/Users/your-user/.config/" and create "powershell" folder and paste the files there
4. now open your windows terminal and type `nvim $PROFILE.CurrentUserCurrentHost` and press `ctrl C` and type `:wq` to save and close neovim
5. type "a" to edit file, paste this code `. $env:USERPROFILE\.config\powershell\user_profile.ps1`
