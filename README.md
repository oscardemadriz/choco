# choco
For Install, open cmd.exe as admin and run:

@"%SystemRoot%\System32\WindowsPowerShell\v1.0\powershell.exe" -NoProfile -InputFormat None -ExecutionPolicy Bypass -Command " [System.Net.ServicePointManager]::SecurityProtocol = 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))" && SET "PATH=%PATH%;%ALLUSERSPROFILE%\chocolatey\bin"

Basic:  

choco install git python nodejs slack vscode yarn googlechrome 7zip.install vlc -y --ignore-checksums

choco install ngrok docker-desktop postman zoom hxd heidisql adobereader dbeaver insomnia-rest-api-client -y --ignore-checksums

cocho install terraform -version 0.12.29

choco install spotify

#Install AWS EB

pip install awsebcli --upgrade --user
