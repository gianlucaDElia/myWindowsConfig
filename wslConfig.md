#WSL Configuration

Install wsl:
```
wls --install
```

Update wsl:
```
wsl --shutdown
wsl --update
```

Open Ubuntu and update packages:
```
sudo apt update
sudo apt upgrade
```

Check if nvidia driver is installed and available:
```
nvidia-smi
```

Remove bell:
Uncomment in /etc/inputrc the line: set bell-style none

Install general pachages:
```
sudo apt install build-essential cmake ninja-build vim nvidia-cuda-toolkit
```

#vcpkg
Install general pachages:
```
sudo apt install zip unzip pkg-config
```

