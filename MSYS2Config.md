# MSYS2 Configurations

Update:
```
pacman -Syu
```

Install toolchain:
```
pacman -S mingw-w64-x86_64-toolchain
```

Install compilers:
```
pacman -S mingw-w64-x86_64-cmake
pacman -S mingw-w64-x86_64-ninja
```

Install fftw:
```
pacman -S mingw-w64-x86_64-fftw
```

Install boost
```
pacman -S mingw-w64-x86_64-boost
```

Install glfw
```
pacman -S mingw-w64-x86_64-glfw
```

Install glew
```
pacman -S mingw-w64-x86_64-glew
```
Dbs
```
pacman -S mingw-w64-x86_64-leveldb
pacman -S mingw-w64-x86_64-db
pacman -S mingw-w64-x86_64-hdf5
```

Language server
```
pacman -S mingw-w64-x86_64-clang
pacman -S mingw-w64-x86_64-clang-tools-extra
```

Dlib
```
pacman -S mingw-w64-x86_64-dlib
```

In stall all in one line:
```
pacman -S mingw-w64-x86_64-toolchain mingw-w64-x86_64-cmake mingw-w64-x86_64-ninja mingw-w64-x86_64-fftw mingw-w64-x86_64-boost mingw-w64-x86_64-leveldb mingw-w64-x86_64-db mingw-w64-x86_64-hdf5 mingw-w64-x86_64-clang mingw-w64-x86_64-clang-tools-extra mingw-w64-x86_64-dlib
```
