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
