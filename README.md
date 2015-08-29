# Hashcat utility

Some old computers can't use the new drivers of NVidia and/or Catalyst.
So, in order to use the ancient versions of Hashcat (and oclXXX-plus),
some changes are required.

This small C code, compiled with -fPIC -shared makes some magic to the
program old versions and makes them active again.
