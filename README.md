# SH-HCC

Write scripts in C language using the GCC compiler.

## Help

hcc

    Usage: hcc [OPTIONS...] FILE ARGUMENTS
    
    This program helps creating script in the C language. A hello world
    script named "hello-world" looks like this:
    
        #if 0 /*
            exec hcc [OPTS...] "hcc" "$@"
            */
        #endif
        #include <stdio.h>
        int main (int argc, const char *argv[]) {
            printf("Hello world.\n");
            return 0;
        }
    
    Options:
    
        -v              : Show used compiler etc.
        -W<arg>         : Add flag.
        -l<LIB> -L<DIR> : Add libraries to link.
        -I<INCDIR>      : Add include directory.
        -S<SOURCE>      : Compile this source.
        -std=<STANDARD> :

## Collaborating

For making bug reports, feature requests and donations visit one of the
following links:

1. [gemini://harkadev.com/oss/](gemini://harkadev.com/oss/)
2. [https://harkadev.com/oss/](https://harkadev.com/oss/)

