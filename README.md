# Stupid Hackathon 2025 prep

Project:
SHA256 Collision Generator


Resources:
- [Inverting XORs](https://www.youtube.com/watch?v=XDsYPXRCXAs&t=597s)
- [XOR swap](https://en.wikipedia.org/wiki/XOR_swap_algorithm)
- SHA256 algorithm [explanation](https://sha256algorithm.com/)
- [sha256.js](https://raw.githubusercontent.com/dmarman/sha256algorithm/refs/heads/main/src/classes/sha.js)

## The Idea


**Input:**
- Pick a block size to limit search range
- Plaintext to encrypt


**Process:**

- Start with the hash digest
- Reverse XOR, ROTR, AND, and OR operations performed by the SHA256
- Whenever data is lost from a ROTR bitwise operation split the guess up and remember all alternatives


**Output:** all the plaintexts that cause collision with the plaintext input


**Extra:** Sort by readability (like [dcode](https://dcode.fr/) does)

