# BLAKE3 Python implementation for UT Algorithmics course project

## Introduction 
BLAKE3 (https://blake3.io/) is a cryptographic hash function, released in 2020, that is designed to be consistenly fast on all platforms, easy to use and implement, and secure

The goal of this project was to implement BLAKE3 in Python, while retaining the speed and security promised by it's designers. 
        
Implementing a cryptographic hash function properly is non-trivial as the algorithm works at a very low-level and the security properties should still hold. This means that any language peculiarities and deviations from the original algorithm have to be thought through carefully and implemented with precision. Additionally, as the function is recent and state-of-art, it is reasonable to assume that even understanding the algorithm might present challenges. 


## Work done
During the length of the project, only the pure hashing mode of BLAKE3 was implemented. While  the  project  implementation  hashes  any  length  inputs  to  any length outputs as intended, it does not give the same hash values as the original BLAKE3 algorithm, indicating possible issues in the security of the implementation.  Furthermore, the project implementation is roughly 1000 times slower than the original Rust implementation on small inputs (n < 1000),  and 10 000 times slower on large inputs (100 000 < n < 10 000 000).  This is due to a severe lack of optimization and the inherent slowness of a purely Python implementation.

A more detailed description of the project is given on the poster.

## Project Author:
Karl Hannes Veskus
