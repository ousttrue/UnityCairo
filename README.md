# UnityCairo

cairo package for Windows(64bit)

## UnityProject

![font extents](font_extents.jpg)

## Dependencies

* zlib: https://www.zlib.net/zlib_license.html
* libpng: src/libpng-1.6.35/LICENSE
* freetype: https://www.freetype.org/license.html
* pixman
* cairo: https://cairographics.org/ LGPL or MPL

## CairoBuild
Build script for cairo.

Below files from [vcpkg](https://github.com/Microsoft/vcpkg). 

* `CairoBuild/cmake/pixman/CMakeLists.txt`
* `CairoBuild/cmake/cairo/CMakeLists.txt`
* `CairoBuild/cmake/cairo/cairo-features.h`

## gen_dllimport.py
This script parse `cairo.h` and generate DllImport code for Unity.
Depends on `libclang.dll` in [llvm](http://releases.llvm.org/).

```
> py -3 -m pip install clang
```

