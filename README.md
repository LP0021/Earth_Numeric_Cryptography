PRNG : EARTH

Round trip encrypt - decrypt script to demonstrate encryption method.
Written in fortran for bitwise processes
Script written with assistance of openAI chatgpt

for seed, use standard 2^random number where random number can be generated from Quantum or standard computing


MMA - Multi Method Approach

For encryption mask :

cos theta sets boundary for the mask on each bit of the array.
if cos theta is greater than 0.7071 set XOR mask on that position, otherwise not. 

cos theta could be calculated by :

(key value / 2^2024 bits ) + ((key value - 2^2024 bits / 2^2024 bits ) x (prime number sequence [first 8 bits of key] x (tan (e^bitposition / e^filesize ))

Or
 
(key value / 2^2024 bits ) - ((key value - 2^2024 bits / 2^2024 bits ) x (fibonnacci number sequence [last 8 bits of key] x (tan (e^bitposition / e^filesize ))

Or 

(key value / 2^2024 bits ) + ((key value - 2^2024 bits / 2^2024 bits ) x (pi number sequence [first 8 bits of key] x (tan (e^bitposition / e^filesize ))

Or 
(key value / 2^2024 bits ) + ((key value - 2^2024 bits / 2^2024 bits ) x (sin[last 8 bits of key] x (tan (e^bitposition / e^filesize ))



With 4 sets of possible encryptions chosen depending on original file and the key, where the value of the first 8bits of the sum is checked: if closer to 256 then its method 1, if closer to 196 then method 2, closer to 126 method 3 and closer to 64 method 4.

The downside is that to decrypt, it seems all 4 methods would have be to tested to find a matching sequence.
 

A second loop could modify the first/last bit selection by computing a value normalized to 2048 depending on both key and first loop iteration to provide a location of a root2048 grid which would be the 8 bit value of key on the modifier.

This might alter standard header data packets for standardised file formats.

Ethos:
LFSR speed using XOR , (tan (e^bitposition / e^filesize )) guarding against encryption pattern identification algorithms.


AI suggested further reading:
Bruce Schneier, Applied Cryptography

Alfred J. Menezes, Paul C. van Oorschot, Scott A. Vanstone, Handbook of Applied Cryptography

D. Bernstein, The Poly1305-AES & ChaCha20 Ciphers

National Institute of Standards and Technology (NIST) SP 800-90A (DRBG standards)

Rueppel, R. «Stream Ciphers,» in Handbook of Cryptography (1995): classic survey of LFSR theory.

Golomb, S. Shift Register Sequences (1982): foundational text on LFSR structure and statistics.
Marsaglia, G. “Xorshift RNGs.” Journal of Statistical Software 8(1) (2003).

Vigna, S. “An experimental exploration of Marsaglia’s xorshift generators, scrambled.” arXiv neural-computing (2016).

Bernstein, D. “ChaCha, a variant of Salsa20.” Workshop Record of SASC (2008).

Gueron, S., et al. “High-Performance AES on x86.” CRYPTO (2011): benchmarks including ChaCha20 vs AES.

Schneier, B. Applied Cryptography (1996): accessible descriptions of LFSR combos and stream ciphers.

Robshaw & Billet (eds.), New Stream Cipher Designs: The eSTREAM Finalists (2008): deep dive into modern, secure, high-performance stream ciphers.

NIST SP 800-90A Rev. 1: guidelines for DRBGs and PRNG constructions.

AI review:
The script is good as a toy or for non-sensitive use. LFSR weakness highlighted. Written to create modulation that might bring speed of XOR with the aim to achieve three step complexity.

Note to thank for the inspiration from the inspirational. 

Disclaimer: 
This is a demo toy and provides no guarantee to the safeguard of encrypted information against threats.
