# Hashcat utility

Some old computers can't use the new drivers of NVidia and/or Catalyst.
So, in order to use the ancient versions of Hashcat (and oclXXX-plus/cudaXXXX-plus),
some adjusments are required.

This small C code, compiled with "-fPIC -shared" makes some magic to the old
program versions and makes them active again.

UPDATE: For a better performance, compile it with "-fPIE -shared". This reduces the
execution time.

## How to use the program:

After the compilation, open a terminal and type:

LD_PRELOAD=./time.so <folder_of_oclXXX-plus>/./oclHashcat-plus.bin
or
LD_PRELOAD=./time.so <folder_of_cudaXXX-plus>/./cudaHashcat-plus.bin

And then you will be able to run the program like in 1970 without changing the system date or
cracking the program (0x71).
