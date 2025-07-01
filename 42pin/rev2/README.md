# Using the adapter in different Amiga boards

1. The 42 pin adapter designed mostly for A1200 boards but it can be used in A500 boards as well.
2. Take care about A18 and A19 address inputs of the adapter. In case of 1MiB Flash ROM typically Kickstart ROM can be programmed to two locations: 0x00000 and 0x80000 to let KS start regardless of A18 state.


