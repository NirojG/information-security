# h5 Uryyb, Greb!
## Chapter1: Foundations (Summary) 

- An encryption is a process of disguising a message in such a way that we can hide its contents or substance and usually for any eavesdropper cannot read the message.
- An encrypted message is a ciphertext.
- Decryption means it is reversing the ciphertext into readable message and recover the message sucessfully from the encryption.
- The science and art of keeping the messages secure is cryptography. 
- Cryptology is the branch of mathmatics encompassing both cryptopraphy and cryptanalysis.
- The practitioners of the cryptology are called crytologists.
- plaintext is denoted by M, for message, or P, for plaintext.

## PGP - Send Encrypted and Signed Message (Summary)
- PGP is used to send secret messages over untrusted internet using encryptions and digital signatures.
- Encryption prevents unauthorized people reading the message, while the signing protects the message for being modified and also it proves the identity of the sender.
- The gpg is an acronym for "GNU privacy guard" which is a popular tool to encrypt and sign.
- We are probably already depending on this tool as Linux kernel development uses PGP signatures.
- A keypair consists of a public key and a private key.
- A public key means which can be shared publicly to encrypt the messages.
- A private key means which must be kept secretly to decrypt the messages.
- we use gpg in command-line and gpg --gen-key is used to create a new identity, where as --export--armor convert the keys to shareable text format.
- In the article to send the secure message, alice encrypts it using tero's public key and signs it with her own private key.
- Tero finally decrypts the message while using his own private key and also he verifies the signature using alice's public key to confirm that it actually did came from her.
- In the article I also learned that if gpg-agent fails during key generation, the process can usually be fixed by running another command which is killall gpg-agent.

## Install OpenSSH server & connecting to it using 'ssh' client 
