# Installation and configuration
Clone the repo
```
git clone https://github.com/Microsoft/vcpkg.git
```
Run the booststrap script (disable telemetry)
```
.\vcpkg\bootstrap-vcpkg.bat -disableMetrics
```
Integrate vcpkg with Visual Studio
```
vcpkg integrate install
```

# FFTW
```
vcpkg.exe install fftw3[threads]:x64-windows
```

fftw3 provides CMake targets:
```
    # this is heuristically generated, and may not be correct
    find_package(FFTW3 CONFIG REQUIRED)
    target_link_libraries(main PRIVATE FFTW3::fftw3)

    find_package(FFTW3f CONFIG REQUIRED)
    target_link_libraries(main PRIVATE FFTW3::fftw3f)

    find_package(FFTW3l CONFIG REQUIRED)
    target_link_libraries(main PRIVATE FFTW3::fftw3l)
```

# Leveldb
```
vcpkg.exe install leveldb:x64-windows
```
```
leveldb provides CMake targets:

    # this is heuristically generated, and may not be correct
    find_package(leveldb CONFIG REQUIRED)
    target_link_libraries(main PRIVATE leveldb::leveldb)
```

# Berkeley
```
vcpkg.exe install berkeleydb:x64-windows
```

# Boost
```
vcpkg.exe install boost:x64-windows
```
