# premake-ninja

Premake extension to support Ninja, because it's awesome.

### Implementation

For each project - configuration pair we create separate .ninja file. For solution we create build.ninja file which imports other .ninja files with subninja command.

Build.ninja file sets phony targets for configuration names so you can build them from command line. And default target is a first configuration name in your project (usually default).  

### TODO

- ninja escaper is not implemented
- gcc toolchain is not supported
- clang toolchain is not supported
- PCH not supported
- Resources are not supported
- Custom build rules are not supported 
- Makefile not supported
- Bundles of any sort are not supported
- Clear methods are not supported 

### Tested on

- msvc / win
	- ConsoleApp works
	- WindowedApp works 
	- StaticLib works
	- SharedLib works
	- win64 not tested
- clang / win
	- not tested
- clang / linux
	- not tested
- clang / os x
	- not tested
- gcc / win
	- not tested
- gcc / linux
	- not tested
