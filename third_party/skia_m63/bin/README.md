# skia tools

- auto compile tools
	- [python2.7](python-2.7.15.amd64.msi)
	- [gn](gn.exe)
	- [ninja](ninja.exe)

- use ninja compile
	- set env path, run [SetToolPath.bat](SetToolPath.bat)
	- generate vs2015 project: 
```
bin\gn.exe gen vs2015\ninja-Static --ide="vs2015" --sln="skia" --args="is_official_build=false skia_use_angle=true angle_use_commit=false skia_use_egl=false skia_enable_spirv_validation=false target_cpu=\"x64\""
```
	- start vs2015: 
```
start vs2015\ninja-Static\skia.sln
```
	- compile and run SampleApp project


