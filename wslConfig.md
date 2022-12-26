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

Unregister ubuntu
```
wsl --unregister Ubuntu
```

Check if nvidia driver is installed and available:
```
nvidia-smi
```

Remove bell:
Uncomment in /etc/inputrc the line: set bell-style none

Install general pachages:
```
sudo apt install build-essential cmake ninja-build gfortran mesa-utils
```

Update to the lates Ubuntu. Change lts to normal in /etc/update-manager/release-upgrade then
```
sudo do-release-upgrade
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

## Cern Root
Install required dependencies [root website](https://root.cern/install/dependencies/)
```
sudo apt install dpkg-dev cmake g++ gcc binutils libx11-dev libxpm-dev \
libxft-dev libxext-dev python-is-python3 libssl-dev gfortran libpcre3-dev \
xlibmesa-glu-dev libglew-dev libftgl-dev \
libmysqlclient-dev libfftw3-dev libcfitsio-dev \
graphviz-dev libavahi-compat-libdnssd-dev \
libldap2-dev python-dev-is-python3 libxml2-dev libkrb5-dev \
libgsl0-dev qtwebengine5-dev
```
Other libraries suggested by [Gabriele Sirri UNIBO](https://www.unibo.it/sitoweb/gabriele.sirri2/contenuti-utili/df5f946d)
```
sudo apt install libtiff5 x11-apps libtbb-dev libgsl0-dev
```
Then unpack and source
```
tar -xzvf root...
source /root/bin/thisroot.sh
```
add the source command to the end of .bashrc
