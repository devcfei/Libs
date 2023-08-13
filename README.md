# Libs

Usefull libraries

## libevent

`Repository` - https://github.com/libevent/libevent

`Building` - by cmake

> cmake -S . -B build32 -DEVENT__LIBRARY_TYPE=STATIC -A Win32
>
> cmake --build build32 --config Release
>
> cmake -S . -B build64 -DEVENT__LIBRARY_TYPE=STATIC -A x64
>
> cmake --build build64 --config Release

`Packaging`

Target | Source
---|---
libevent/include | libevent/include + build/include
libevent/lib/x86 | libevent/build32/lib/Release
libevent/lib/x64 | libevent/build64/lib/Release
