# Beaver's C++ Library

This is my personal C++ library. I started writing it when C++11 was considered fresh and new, so most parts are intended as replacement or extensions for clumsy old-C++ libraries. C++17 or even C++20 have many features that make parts of this library obsolete. I also do a lot of things with CUDA, so part of this library is dedicated to GPU programming.

You may use this library at your convenience for noncommercial projects -- the code is available under CC 3.0 BY-NC (http://creativecommons.org/). The code is presented as is with no warranties whatsoever.

The library is header-only, so all you need to do is to add the `include` directory in your compilation path. The `tests` and `cuda_tests` are projects used to test the library and demonstrate its utilization. Both projects are part of Microsoft Visual Studio solution and they have good ol' Makefiles, so they can be compiled easy enough on Windows and Linux.
