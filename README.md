```cpp
#ifdef CEXPORT
#define Giris __attribute__((constructor)) \
                   void __constructor ()
#else
#define Giris int main ()
#endif

#define Selam printf("Selam! ben Poyraz.\n")

#include <cstdio>

Giris {
    Selam;
}

// main.cpp
// gcc main.cpp -o vureone && ./vureone
```
