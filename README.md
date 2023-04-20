# choco
For Install, open cmd.exe as admin and run:

@"%SystemRoot%\System32\WindowsPowerShell\v1.0\powershell.exe" -NoProfile -InputFormat None -ExecutionPolicy Bypass -Command " [System.Net.ServicePointManager]::SecurityProtocol = 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))" && SET "PATH=%PATH%;%ALLUSERSPROFILE%\chocolatey\bin"

Basic:  

> choco install slack vscode googlechrome 7zip.install vlc adobereader zoom zoomit oh-my-posh -y --ignore-checksums

Basic Developer:

> choco install git python nodejs yarn docker-desktop nvm -y --ignore-checksums
 
Developer +:

> choco install ngrok postman  hxd heidisql  dbeaver insomnia-rest-api-client -y --ignore-checksums 

Amazon:

> choco install terraform -version 0.12.29
> 
> pip install awsebcli --upgrade --user


Why not:
> choco install spotify
> 
> choco install sharex autohotkey fsviewer -y --ignore-checksums

#Install AWS EB

pip install awsebcli --upgrade --user

# Oh my posh theme

```
Install-Module -Name Terminal-Icons -Repository PSGallery
mkdir ~/oh-my-posh-theme
Invoke-WebRequest -OutFile ~/oh-my-posh-theme/mytheme.omp.json -Uri https://raw.githubusercontent.com/oscardemadriz/choco/master/.atomiccustom.omp.json
echo "oh-my-posh init pwsh --config '~/oh-my-posh-theme/mytheme.omp.json' | Invoke-Expression" > $PROFILE
```

Nerd font:
 `https://github.com/ryanoasis/nerd-fonts/releases/download/v2.1.0/FiraCode.zip`

Configurar en Terminal > Powershell > Apariencia > Fuente > FiraCode


# MacOS

Basic:

```
brew install --cask slack
brew install --cask visual-studio-code
brew install --cask google-chrome
brew install --cask 7zip
brew install --cask vlc
brew install --cask adobe-acrobat-reader
brew install zoomit
```

Developer:

```
brew install git
brew install python
brew install node
brew install yarn
brew install --cask docker
brew install nvm
brew install --cask ngrok
brew install --cask postman
brew install hxd
brew install --cask dbeaver-community
```

Why not: 

```
brew install --cask spotify
brew install --cask loom
```


# Git

## .gitconfig

```
[core]
	autocrlf = input
	eol = lf
[alias]
st = status
co = checkout
aa = add --all
m = commit -m 
amen = commit --amend
cagada = reset HEAD~1
nuke = reset --hard HEAD
wip = commit -m 'WIP' --no-verify
publish = !git push --set-upstream origin $(git branch | grep '*' | sed 's/* //')
```
