# verious urls

* [A stackoverflow blog? on GenAI](https://stackoverflow.blog/2023/10/09/from-prototype-to-production-vector-databases-in-generative-ai-applications/)


# non germain url

Found this regarding fortran:

```
See:
   https://en.wikipedia.org/wiki/RANDU

Here is the original FORTRAN code for the subroutine named "RANDU" -- first documented in the IBM Scientific Subroutine Package (SSP) for S/360 ...

        SUBROUTINE RANDU(IX,IY,YR)
        IY=IX*65539
        IF(IY)5,6,6
 5      IY=IY+2147483647+1
 6      YR=IY
        YR=YR*.4656613E-9
        RETURN
        END

NOTE:  RANDU can be improved somewhat by substituting "69069" in place of "65539" as the modulo.

You can compile this with IBM's FORTRAN G or H compiler and request the option to see the generated assembler language code, and you should be able to extract what you need.

That should get you started ...
```

* [s370asm](https://groups.io/g/hercules-s370asm)
* [bal sieve](http://cs.ecs.baylor.edu/~maurer/SieveE/bal.htm)
* [bal wiki](https://en.wikipedia.org/wiki/Sieve_of_Eratosthenes)
* [S370BALAsm](https://github.com/SYSPROG-JLS/S370BALAsm)
* [S370BALEmulator](https://github.com/SYSPROG-JLS/S370BALEmulator)




