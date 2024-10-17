Here's the integrated OSINT and Cryptography section, with all relevant resources and hashes included:

---

## OSINT (Open Source Intelligence)

If I get an OSINT question, what can I do? Depending on the question, you may:

- **Just look it up!**
- **Find metadata:** [Metadata2Go](http://metadata2go.com/)
- **HTTP Headers questions:** [HTTP Header Fields](https://en.wikipedia.org/wiki/List_of_HTTP_header_fields#Request_fields)
- **Website registration data lookup:** [ICANN Lookup](https://lookup.icann.org/en)
- **PGP Lookup Database:**
  - [Ubuntu PGP Keyserver](http://keyserver.ubuntu.com/)
  - [OpenPGP Keyserver](http://keys.openpgp.org/)
  - [MIT PGP Keyserver](http://pgp.mit.edu/)
- **SSL Verification:** Check the lock icon > Connection is secure > Certificate is valid
- **Analyze:** [Online Barcode Reader](https://online-barcode-reader.inliteresearch.com/)

## Cryptography

If I encounter a cryptography-related question, I can:

- **Use converters:** [RapidTables Number Conversion](https://www.rapidtables.com/convert/number/index.html) (may be used for different number conversions, but not recommended)
- **Understand types of encryption.**
- **Explore hidden messages in images:**
  - Option 1: `strings Steg1.jpg | grep SKY`
  - Option 2: [Examine image metadata for hidden data.](http://metadata2go.com/)
  - Option 3: Use Steganography
    - [Osrich Steg Decoder](https://osric.com/chris/steganography/decode.html)
    - [GeorgeOm](https://georgeom.net/StegOnline/upload)

### Common Hashes and Their Examples

1. **MD5**
   - **Example**: `5d41402abc4b2a76b9719d911017c592` (hash of "hello")
   - **Solving**: Use hash lookup features.

2. **SHA-1**
   - **Example**: `f5d3b4f7a62c1a4e4f2a0b3f68a3f0d7d5c1d0df` (hash of "hello world")
   - **Solving**: Similar methods as MD5.

3. **SHA-256**
   - **Example**: `6c1b1e4f9dffb6f2b1f03f7e6c1c13c8b1b1f6f7f3f0e17b9f3f7e6c1c1c1c1`
   - **Solving**: Same approach as MD5.

4. **SHA-512**
   - **Example**: `cf83e1357eefb8bdf1542850d66d8007d62085f7d1f1e6ff0f5c90f6ab6a7b7a5a4f5e3d3e6cd5ed6c1c0e0e5d3a5c8c0071b4bf0c3c1c3b4c3c3c3e5a5b5e5f`
   - **Solving**: Same as above.

5. **bcrypt**
   - **Example**: `$2b$12$eImiTXuWVxfM37uY4JANjOa5z1U2d8L3c1Q1W9Fh3k2oJ3pF1sW1y`
   - **Solving**: Use bcrypt cracking tools.

### Less Common Hashes

6. **Whirlpool**
   - **Example**: `c5a9c4c1e5c9b2f9d5c1e7c1ff9e1d2c1b5e4f7c1e3b6c8f1d5c7f0e9f3b1c3`
   - **Solving**: Use the "Whirlpool" operation.

7. **Tiger**
   - **Example**: `3299A0C0D55E0E91F9D0A8C0F9A0A0F3A0B1B2F1`
   - **Solving**: Use hash lookup.

8. **RIPEMD-160**
   - **Example**: `c8c3e4d5f7d1e8a7b9e1d2c4f3e1d2c1f4e5c6e7`
   - **Solving**: Use hash operations in CyberChef or dCode.

### Common Encryption Methods

9. **RSA (Rivest-Shamir-Adleman)**
   - **Example**: 
     - **Public Key**: `n = 2537, e = 13`
     - **Ciphertext**: `855`
   - **Solving**:
     - **CyberChef**: Use "RSA Decrypt," providing the private key derived from the public key.
     - **dCode**: Use the RSA decryption tool.

10. **ElGamal**
    - **Example**: 
      - **Public Key**: `p = 23, g = 5, y = 18`
      - **Ciphertext**: `(k = 15, c1 = 19, c2 = 20)`
    - **Solving**: Use ElGamal decryption tools.

11. **DSA (Digital Signature Algorithm)**
    - **Example**: 
      - **Public Key**: `(p, q, g, y)`
      - **Signature**: `(r, s)`
    - **Solving**: Typically used for verification.

### Additional Ciphers and Encodings

12. **Caesar Cipher**
    - **Example**: `Khoor Zruog` (shift of 3 for "Hello World")
    - **Solving**: Use the "Caesar Cipher" operation.

13. **Vigenère Cipher**
    - **Example**: `Lxfopv ef rnhr` (using key "LEMON")
    - **Solving**: Use the "Vigenère Cipher" operation.

14. **ROT13**
    - **Example**: `Uryyb Jbeyq` (decodes to "Hello World")
    - **Solving**: Use "ROT13".

15. **AES (Advanced Encryption Standard)**
    - **Example**: Encrypted text: `3D3A4D4E44AAB8D0C4F1A8D2F8D3E4C7`
    - **Solving**: Use "AES Decrypt" operation with key and IV.

16. **XOR Cipher**
    - **Example**: `48656c6c6f` XOR with key `key`
    - **Solving**: Use the "XOR" operation.

17. **Base64**
    - **Example**: `SGVsbG8gV29ybGQ=` (decodes to "Hello World")
    - **Solving**: Use "From Base64".

18. **Hexadecimal**
    - **Example**: `48656c6c6f` (decodes to "Hello")
    - **Solving**: Use "From Hex".

19. **URL Encoding**
    - **Example**: `Hello%20World` (decodes to "Hello World")
    - **Solving**: Use "URL Decode".

20. **Morse Code**
    - **Example**: `.... . .-.. .-.. ---` (decodes to "HELLO")
    - **Solving**: Use "Morse Code".

21. **Playfair Cipher**
    - **Example**: `CIPHERTEXT` (with key "KEYWORD")
    - **Solving**: Use Playfair cipher tools.

22. **Atbash Cipher**
    - **Example**: 
      - **Plaintext**: `HELLO`
      - **Ciphertext**: `SVOOL` (each letter is replaced with its opposite: A ↔ Z, B ↔ Y, etc.)
    - **Solving**:
      - **CyberChef**: Use "Atbash Cipher".
      - **dCode**: Use the Atbash cipher tool.

### Rail Fence Cipher and Similar Ciphers

23. **Rail Fence Cipher**
    - **Example**: 
      - **Plaintext**: "HELLO WORLD"
      - **Ciphertext**: `HLOOL ELWRD` (with 2 rails)
    - **Solving**:
      - **CyberChef**: Use the "Rail Fence Cipher" operation and specify the number of rails.
      - **dCode**: Use the Rail Fence cipher tool.

24. **Columnar Transposition Cipher**
    - **Example**: 
      - **Plaintext**: "HELLO WORLD"
      - **Key**: `3142` (rearranging columns)
      - **Ciphertext**: `HLOEL WDOR`
    - **Solving**:
      - **CyberChef**: Use "Columnar Transposition" and provide the key.
      - **dCode**: Use the Columnar transposition tool.

25. **Scytale Cipher**
    - **Example**: 
      - **Plaintext**: "HELLO WORLD"
      - **Key**: `3` (diameter of the rod)
      - **Ciphertext**: `HLOOL ELWRD`
    - **Solving**:
      - **CyberChef**: Use "Scytale Cipher" and specify the key length.
      - **dCode**: Use the Scytale cipher tool.

## Password Cracking

### Hashcat

#### Hashcat is a robust password recovery tool that supports various hash types and cracking modes.

Usage Example:
- Cracking MD5 Hashes: `hashcat -a 0 -m 0 hashes.txt wordlist.txt`
- Cracking SHA1 Hashes: `hashcat -a 0 -m 100 hashes.txt wordlist.txt`
- Cracking bcrypt Hashes: `hashcat -a 0 -m 3200 hashes.txt wordlist.txt`

Commonly Used Options:
- `-a`: Attack mode (0 for straight, 1 for combination, etc.)
- `-m`: Hash type (0 for MD5, 100 for SHA1, 3200 for bcrypt)
- `-o`: Output file for cracked hashes

Resources:
- [Hashcat Documentation](https://hashcat.net/wiki/)
- [Hashcat GitHub Repository](https://github.com/hashcat/hashcat)


### JohnTheRipper
#### John the Ripper is a fast password cracker, currently available for many flavors of Unix, macOS, Windows, DOS, BeOS, and OpenVMS.

Usage Example:
- Cracking MD5 Hashes: `john --format=raw-md5 hashes.txt --wordlist=wordlist.txt`
- Cracking SHA1 Hashes: `john --format=raw-sha1 hashes.txt --wordlist=wordlist.txt`
- Cracking bcrypt Hashes: `john --format=bcrypt hashes.txt --wordlist=wordlist.txt`
- Commonly Used Options
`--format`: Specify the hash type (raw-md5 for MD5, raw-sha1 for SHA1, bcrypt for bcrypt)
`--wordlist`: Specify the wordlist file to use for cracking
`--rules`: Apply wordlist rules to modify words

Resources:
- [John the Ripper Documentation]()
- [John the Ripper GitHub Repository]()

### Windows NTLM password cracking
TODO
