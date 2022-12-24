# WSL Configuration

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
sudo apt install build-essential cmake ninja-build gfortran
```

## vcpkg
Install general pachages:
```
sudo apt install zip unzip pkg-config
```

Clone the vcpkg repo
```
cd /opt
sudo git clone https://github.com/Microsoft/vcpkg.git
```

Run the bootstrap script to build vcpkg
```
sudo ./opt/vcpkg/bootstrap-vcpkg.sh
```
