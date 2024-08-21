## Install git
```
curl -L -o git-installer.exe https://github.com/git-for-windows/git/releases/download/v2.42.0.windows.1/Git-2.42.0-64-bit.exe
powershell -Command "Invoke-WebRequest -Uri 'https://github.com/git-for-windows/git/releases/download/v2.42.0.windows.1/Git-2.42.0-64-bit.exe' -OutFile 'git-installer.exe'"
git-installer.exe /SILENT /NORESTART
set PATH=%PATH%;C:\Program Files\Git\cmd
git --version
```

## Install python3
```
curl -L -o python-installer.exe https://www.python.org/ftp/python/3.11.4/python-3.11.4-amd64.exe
powershell -Command "Invoke-WebRequest -Uri 'https://www.python.org/ftp/python/3.11.4/python-3.11.4-amd64.exe' -OutFile 'python-installer.exe'"
python-installer.exe /quiet InstallAllUsers=1 PrependPath=1
set PATH=%PATH%;C:\Program Files\Python311
set PATH=%PATH%;C:\Program Files\Python311\Scripts
python --version
```
