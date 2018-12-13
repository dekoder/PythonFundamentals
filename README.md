# Python Fun(dementals)

# setup guide

## Windows 10
You will need Chocolatey, this can be installed easily with a one-line download:\
```cmd
@"%SystemRoot%\System32\WindowsPowerShell\v1.0\powershell.exe" -NoProfile -InputFormat None -ExecutionPolicy Bypass -Command "iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))" && SET "PATH=%PATH%;%ALLUSERSPROFILE%\chocolatey\bin"
```
NOTE: Install guide can be found here [https://chocolatey.org/docs/installation#installing-chocolatey](https://chocolatey.org/docs/installation#installing-chocolatey)
```powershell
choco install -y python vscode git cmder
python -m pip install -U pip
pip install --user --upgrade pipenv
```
You may need to add pipenv to your path (Ex. here was my path):
```
C:\Users\Killswitch3\AppData\Roaming\Python\Python36\Scripts
```
Now our enviroment is ready to to start to get to work within powershell:
```powershell
PS C:\Users\Killswitch3\tools> git clone https://github.com/obscuritylabs/PythonFundamentals.git 
PS C:\Users\Killswitch3\tools> cd .\PythonFundamentals\
PS C:\Users\Killswitch3\tools> python -m pipenv install
PS C:\Users\Killswitch3\tools> python -m pipenv shell
```

## MacOS
You will need Homebrew which is a package manager for MacOS.:
```bash
xcode-select --install
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```
NOTE: Install guide can be found here [https://brew.sh/](https://brew.sh/)
```bash
alexanderrymdeko-harvey@alexandersMBP2:~/tools/PythonFundamentals$  brew install python3 pipenv git
alexanderrymdeko-harvey@alexandersMBP2:~/tools/PythonFundamentals$  python3 -m pip install -U pip
```
Now our enviroment is ready to to start to get to work within Terminal:
```bash
alexanderrymdeko-harvey@alexandersMBP2:~/tools$ git clone https://github.com/obscuritylabs/PythonFundamentals.git
alexanderrymdeko-harvey@alexandersMBP2:~/tools$ cd PythonFundamentals
alexanderrymdeko-harvey@alexandersMBP2:~/tools/PythonFundamentals$ pipenv install 
alexanderrymdeko-harvey@alexandersMBP2:~/tools/PythonFundamentals$ pipenv shell
(PythonFundamentals) alexanderrymdeko-harvey@alexandersMBP2:~/tools/PythonFundamentals$ python --version
Python 3.6.6
```
## Ubuntu 18.04
You will need apt, but ubuntu is easy...
```bash
sudo apt update && apt install -y python3 python3-dev python3-pip 
python3 -m pip install -U pip
sudo pip3 install --user --upgrade pipenv
```
