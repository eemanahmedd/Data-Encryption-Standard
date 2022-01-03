# Data-Encryption-Standard

DES is the most widely used encryption scheme. It is a **block cipher** algorithm. The plaintext is processed in 64-bit blocks, and the key is 56-bits in length; generated orignally from_ 64-bits_.

Since it’s a symmetric-key algorithm, it employs the same key in both encrypting and decrypting the data. 


**DES Algorithm Steps**


The algorithm process breaks down into the following steps:
- The process begins with the 64-bit plain text block getting handed over to an initial permutation (IP) function.
- The initial permutation (IP) is then performed on the plain text.
- Next, the initial permutation (IP) creates two halves of the permuted block, referred to as Left Plain Text (LPT) and Right Plain Text (RPT).
- Each LPT and RPT goes through 16 rounds of the encryption process.
- Finally, the LPT and RPT are rejoined, and a Final Permutation (FP) is performed on the newly combined block.
- The result of this process produces the desired 64-bit ciphertext.

The encryption process step (step 4, above) is further broken down into five stages:
- Key transformation
- Expansion permutation
- S-Box permutation
- P-Box permutation
- XOR and swap

**For decryption, we use the same algorithm, and we reverse the order of the 16 round keys.**__
