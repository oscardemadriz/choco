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

`oh-my-posh init pwsh --config 'https://raw.githubusercontent.com/oscardemadriz/choco/master/.atomiccustom.omp.json' | Invoke-Expression` 

`Install-Module -Name Terminal-Icons -Repository PSGallery`

Nerd font:
 `https://github.com/ryanoasis/nerd-fonts/releases/download/v2.1.0/FiraCode.zip`
