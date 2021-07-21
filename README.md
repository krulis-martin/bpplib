# Beaver's C++ Library

This is my personal portable C++ library. I started writing it when C++11 was considered fresh and new, so most parts were intended as replacement or extensions for clumsy old-C++ libraries. C++11 (and newer) have many features that make parts of this library obsolete. I also do a lot of things with CUDA, so part of this library is dedicated to GPU programming.

You may use this library (or any part independently) at your convenience for noncommercial projects -- the code is available under CC 3.0 BY-NC (http://creativecommons.org/). The code is presented as is with no warranties whatsoever.

The library is header-only, so all you need to do is to add the `include` directory in your compilation path. The `tests` and `cuda_tests` are projects used to test the library and demonstrate its utilization. Both projects are part of Microsoft Visual Studio solution and they have good ol' Makefiles, so they can be compiled easy enough on Windows and Linux.


## Library structure

* `algo` - selected algorithms implemented in templated form (namely k-means and k-medoids clustering, Levenshtein's edit distance, Least Common Substring algorithm, and a few string utilities)
* `cli` - tools for command-line applications (argument processing, logging, and some terminal functions)
* `cuda` - some wrappers that make CUDA programming a little more convenient in C++
* `datastruct` - a few data structures, some of them not completed yet (regular heap, key-value store, and string index should be functional)
* `math` - mathematical utilities (random is obsolete, `<random>` from C++11 is much better choice)
* `misc` - universal exceptions with stream-like interface, ptr_fix (polyfill for `make_unique` and `make_shared` for C++11)
* `para` - C++-only implementation of blocking queue and crude thread pool (in case one needs some parallelism, but OpenMP/TBB are not available)
* `system` - system-related APIs (various files and file system interfaces, info tools, and stopwatch)
