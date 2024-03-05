#DES Encryption and Decryption Program
This program implements the Data Encryption Standard (DES) algorithm for encrypting and decrypting messages. DES is a symmetric-key algorithm, meaning the same key is used for both encryption and decryption.

Features
Encryption: Encrypt plaintext messages using DES algorithm.
Decryption: Decrypt ciphertext messages encrypted using DES algorithm.
Mode: Uses Electronic Codebook (ECB) mode for encryption.
Usage
1. Compilation
Compile the program using a C++ compiler. For example, using g++:

bash
Copy code
g++ -o des des.cpp
2. Running the Program
Run the compiled program des. Upon execution, it will prompt you to input a plaintext message and a secret key (64 bits).

bash
Copy code
./des
Follow the prompts to enter the plaintext message and the secret key.

3. Output
After encryption, the program will display the encrypted ciphertext.

After decryption, the program will display the decrypted plaintext.

Example
Here's an example run of the program:

plaintext
Copy code
Enter plaintext message: Hello, World!
Enter secret key (64 bits): 0110100101010101110101001010100011110101100110100100011100101001

Encrypted ciphertext: 0011011000110110101001100001001000000000000000000000000011110110
Decrypted plaintext: Hello, World!
ECB Mode
Electronic Codebook (ECB) mode is used for encryption. In ECB mode, each block of plaintext is encrypted independently using the same key. This can lead to identical plaintext blocks being encrypted to identical ciphertext blocks.

Notes
The program expects the secret key to be provided as a binary string of 64 bits.
The plaintext message can include spaces and any printable ASCII characters.
Ensure proper handling of the secret key, as it is crucial for the security of the encryption.
