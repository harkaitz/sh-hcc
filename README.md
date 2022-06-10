# SH-HCC

Write scripts in C language using the GCC compiler.

## Help

hcc

    Usage: hcc [OPTIONS...] FILE ARGUMENTS
    
    Launch a C program like if it was a scripting language. The
    bootstrap is done the following way:
    
        #if 0 /*
            exec hcc [OPTS...] "hcc" "$@"
            */
        #endif
        #include <stdio.h>
        int the_script_filename (int argc, const char *argv[]) {
            printf("Hello world.\n");
            return 0;
        }
    
    The following environment variables are used.
    
        Compilation: CC,CFLAGS,CPPFLAGS,LDFLAGS,LIBS,FORCE_BUILD
        Launcher:    HCC_RUN (ie env or nice)
    
    Options:
    
        -v              : Show used compiler etc.
        -W<arg>         : Add flag.
        -l<LIB> -L<DIR> : Add libraries to link.
        -I<INCDIR>      : Add include directory.
        -S<SOURCE>      : Compile this source.
        -std=<STANDARD> : The C standard to use.

## Collaborating

For making bug reports, feature requests and donations visit
one of the following links:

1. [gemini://harkadev.com/oss/](gemini://harkadev.com/oss/)
2. [https://harkadev.com/oss/](https://harkadev.com/oss/)

