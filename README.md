# Compare Performance and complexity of Software Interpreters of a Virtual Machine

Sample programs for comparison of different VM interpretation techniques.
See the Makefile for the full list of targets.

* `switched` - switched interpreter
* `threaded` - threaded interpreter
* `predecoded` - switched interpreter with preliminary decoding phase
* `subroutined` - subroutined interpreter
* `threaded-cached` - threaded interpreter with pre-decoding.
* `tailrecursive` - subroutined interpreter with tail-call optimization
* `translated` - binary translator to Intel 64 machine code
* `native` - a static implementation of the test program in C

Use `./measure.sh` to measure run time of individual binaries or to perform a comparison of all techniques (alternatively, run `make all measure`).

Tested to compile and run with GCC 4.8.1, GCC 5.1.0 and ICC 15.0.3 on Ubuntu Linux 12.04.5. Limited testing was also done on Windows 8.1 Cygwin64 environment, GCC 4.8.

An article discussing structure, performance variations, and comparison of interpreters: http://habrahabr.ru/company/intel/blog/261665/ (in Russian).
