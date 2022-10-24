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
vcpkg.exe install fftw3[avx2,threads,openmp]:x64-windows
```
