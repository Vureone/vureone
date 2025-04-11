```cpp
#ifdef CEXPORT
#define entrypoint __attribute__((constructor)) \
                   void __constructor ()
#else
#define entrypoint int main ()
#endif

#include <cstdio>

entrypoint {
    printf( "Merhaba, ben Poyraz." );
}
```
