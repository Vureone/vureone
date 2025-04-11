```cpp
#ifdef CEXPORT
#define Giris __attribute__((constructor)) \
                   void __constructor ()
#else
#define Giris int main ()
#endif

#define Selam printf("Merhaba! ben Poyraz.")

#include <cstdio>

Giris {
    Selam;
}
```
