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
Using with cmake
```
cmake -B [build directory] -S . -DCMAKE_TOOLCHAIN_FILE=[path to vcpkg]/scripts/buildsystems/vcpkg.cmake
```

# FFTW
```
vcpkg.exe install fftw3[threads,avx2]:x64-windows
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

# HDF5
```
vcpkg.exe install hdf5[cpp,tools,threadsafe]:x64-windows
```
```
# this is heuristically generated, and may not be correct
    find_package(hdf5 CONFIG REQUIRED)
    # note: 1 additional targets are not displayed.
    target_link_libraries(main PRIVATE hdf5::hdf5-shared hdf5::hdf5_hl-shared hdf5::hdf5_cpp-shared hdf5::hdf5_tools-shared)
```

# HIGHFIVE
```
vcpkg.exe install highfive[boost]:x64-windows
```
```
# this is heuristically generated, and may not be correct
    find_package(HighFive CONFIG REQUIRED)
    # note: 1 additional targets are not displayed.
    target_link_libraries(main PRIVATE libdeps HighFive HighFive_libdeps HighFive_HighFive)
```

# Dlib
```
vcpkg.exe install dlib[fftw3]:x64-windows
```
```
# this is heuristically generated, and may not be correct
    find_package(dlib CONFIG REQUIRED)
    target_link_libraries(main PRIVATE dlib::dlib)
```
# openBLAS
```
vcpkg.exe install openblas[threads]:x64-windows
```
```
# this is heuristically generated, and may not be correct
    find_package(OpenBLAS CONFIG REQUIRED)
    target_link_libraries(main PRIVATE OpenBLAS::OpenBLAS)
```
# Matplot++
```
vcpkg.exe install  matplotplusplus[fftw,blas,jpeg,opengl]:x64-windows
```
```
# this is heuristically generated, and may not be correct
    find_package(matplot++ CONFIG REQUIRED)
    target_link_libraries(main PRIVATE Matplot++::cimg std::filesystem Matplot++::matplot Matplot++::nodesoup)
```
# RapidJSON
```
vcpkg.exe install rapidjson:x64-windows
```
```
# this is heuristically generated, and may not be correct
    find_package(RapidJSON CONFIG REQUIRED)
    target_link_libraries(main PRIVATE rapidjson)
```
# VTK
```
vcpkg.exe install vtk[opengl]:x64-windows
```
```
# this is heuristically generated, and may not be correct
    find_package(VTK REQUIRED)
    include("${VTK_USE_FILE}")
    target_link_libraries(main PRIVATE ${VTK_LIBRARIES})
```
