```cpp
#ifdef CEXPORT
#define entrypoint __attribute__((constructor)) \
                   void __constructor ()
#else
#define entrypoint void main ()
#endif

entrypoint {
    printf( "Merhaba, ben Poyraz." );
}
```
