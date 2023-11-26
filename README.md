# VTK Tutorial

VTK tutorial file to be used with VCPKG files. This was a reminder on how to use VTK.

## How to use this

### VCPKG

First you should have VCPKG installed localy on the machine:
- https://github.com/microsoft/VCPKG

Install it by just cloning the repo on your local machine and then running the `.bat` or `.sh` file depending on you OS. 

```pwsh
git clone https://github.com/microsoft/vcpkg.git
.\vcpkg\bootstrap-vcpkg.bat
```

### Back to the repo

You can now clone the local repo and execute it, WARNING this may take some time as it has to rebuild the all VTK dependencies.

```pwsh
git clone https://github.com/anirul/vtktutorial.git
mkdir build
cd build
cmake .. --DCMAKE_TOOLCHAIN_FILE="../../vcpkg/scripts/buildsystems/vcpkg.cmake"
```

You should have a project that has been created for you OS, this could be a `.sln` solution file or a `makefile`.

### Execute the project file

Now you can use the project file to see the project or just make it using the generated `makefile`.
