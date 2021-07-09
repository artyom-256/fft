### Fast Fourier Transformation

Implementation of sequential Cooley–Tukey algorithm for computation of Fourier Transformation. Implementation focused on computation speed by having pre-calculated table of roots of unity, so sacrifying memory. It means the algorithm has limited amount of array sizes to process, in particular: 2, 4, 8, 16, 32, 64, 128, 256. This also makes possible to define fast versions of pow2(), log2() and inv_sqrt() functions with pre-calculated values. Also since we focus on speed, there is no sanity checks, so invoking fft() with unexpected parameters will lead to undefined behaviour.

### Tools:

Just put here tools that I use under Windows. In theory the project should work for a wide variety of compilers.

* MinGW version 7.3.0
* CMake version 3.17.1

### Build:

```
git clone https://github.com/artyom-256/fft.git
cd fft
mkdir build
cd build
cmake ..
# run your favorite compiler here
```
