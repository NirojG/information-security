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

## A) Install OpenSSH server & connecting to it using 'ssh' client 
<img width="820" height="401" alt="image" src="https://github.com/user-attachments/assets/b24ba77e-e9f6-484b-9057-1ef97fd762e1" />
- installed the Openssh server now connecting it to localhost
<img width="961" height="577" alt="image" src="https://github.com/user-attachments/assets/7291dc1a-fc95-4910-b227-3d813ed1d278" />

## B) Automate SSH using public keys 
- Here I did ssh-keygen which creates a key of both public and private key and followed by ssh-copy-id  to copy the generated key to the local host server this allows automation.

<img width="824" height="381" alt="image" src="https://github.com/user-attachments/assets/b89a23b4-200f-4ab1-bece-aa2f378479dd" />

<img width="951" height="725" alt="image" src="https://github.com/user-attachments/assets/7f29c8e9-c6a2-4170-b57a-e68fca0e3b9e" />


- Here the key is added after ssh-copy-id
<img width="963" height="794" alt="image" src="https://github.com/user-attachments/assets/59f1d3a4-a378-4c89-a9d2-be502dc34998" />

- Now trying to log in the localhost without the password via automation, I didn't have to login i directly went inside the localhost without a password.

<img width="961" height="784" alt="image" src="https://github.com/user-attachments/assets/0eb1af0e-f8ad-4436-8783-90a2d3c714bb" />

## C) Password manager: cloudless and free, open source
- For this assignment I choosed KeePassXC which is a free, open-source password manager that operates entirely cloudless, and it helps storing all credentials in a local machine while in a heavily encrypted database file.
- I installed KeePassXC via terminal. sudo apt install keepassxc.
<img width="955" height="547" alt="image" src="https://github.com/user-attachments/assets/d97330f6-ff6b-462c-b8c8-962392e4e781" />

<img width="954" height="761" alt="image" src="https://github.com/user-attachments/assets/49b90839-a0f3-47a0-a288-f6240afb6eed" />

### Demonstration of KeePassXC usage & functionality

- Now openning via applications dropdown menu accessories KeePassXC
<img width="952" height="643" alt="image" src="https://github.com/user-attachments/assets/6b9202e5-f5a6-4dd5-976b-11f795566686" />

-  I create a new database and give name of MyPasswords. I use recommended database format & enter a password to access and protect my database.

<img width="957" height="788" alt="image" src="https://github.com/user-attachments/assets/a03868fc-bce1-41c0-acdc-393ec9bedff3" />

- I saved my password database in desktop where I can access it easily. 
<img width="1290" height="817" alt="image" src="https://github.com/user-attachments/assets/e952df30-8294-4670-805e-de41d9b3fe5b" />

- I added a new entry by clicking the + button and I wrote my account as my title and my name as username. and entered a password.

<img width="956" height="796" alt="image" src="https://github.com/user-attachments/assets/ea2329fb-80e3-488a-9a5e-fb329eeeac71" />

<img width="947" height="793" alt="image" src="https://github.com/user-attachments/assets/9c56dbcd-23fc-49c4-ab68-a1d299f6feec" />

### Why password managers is needed? what kind of attacks or threats it protects against.what kind of attacks or threats it protects against.

- By this way we can safely save any number of passwords in the password manger. We just need the master password i.e. the password manager password to access all our passwords that we have safely and securely saved in our device.
  
- Password managers like KeePassXC protects against bruteforce attacks and other credentials stuffing. It ensures that our every account has always long and unique passwords which are highly improbable to either guess or impossible to crack. 

## D) Pretty Good indeed. Encrypt and decrypt a message with 'gnupg', using PGP public key cryptography.
- First here I used command gpg --full-generate-key
<img width="964" height="675" alt="image" src="https://github.com/user-attachments/assets/0c84d5cb-f2d3-4640-bc6b-5a17b9d379cf" />

- I choosed (1) RSA and RSA
<img width="964" height="796" alt="image" src="https://github.com/user-attachments/assets/62ace1cb-f21a-485a-b450-eb4198c4a763" />

- Then I choosed 3072 for the key size
- And after that I choose 0 key does doesnot expire
<img width="962" height="798" alt="image" src="https://github.com/user-attachments/assets/96274343-ed04-4876-8948-49c2fc31ce5d" />

- I selected yes to my decision and then proceeded to enter my real name and email address to construct a user ID.
 
 <img width="962" height="795" alt="image" src="https://github.com/user-attachments/assets/65563bff-823c-4001-80db-c55aa48f1cae" />

- their was the comment field i left it empty for now.

<img width="957" height="793" alt="image" src="https://github.com/user-attachments/assets/0832a047-d8ab-4cc8-b49a-1e6f829beb8a" />

- I pressed O for confirming my details which is basically Okay and proceeded.
<img width="945" height="799" alt="image" src="https://github.com/user-attachments/assets/d84d796c-f89e-4f95-bda3-ae1ec22a428a" />

- Now we are at the final step of key generation, it is now asking for a Passphrase to protect my new pgp. I entered a password proceeded further 

<img width="964" height="793" alt="image" src="https://github.com/user-attachments/assets/41aa0a1c-4075-4374-8e4e-64f8829e6f6a" />

<img width="963" height="808" alt="image" src="https://github.com/user-attachments/assets/b305985d-33e7-4de8-b4df-572275f30c3e" />

### Encrypting and Decrypting a message with gnupg, using pgp public key cryptography
- Now firstly we create the file named Niroj.txt.
<img width="958" height="801" alt="image" src="https://github.com/user-attachments/assets/2d79fc74-6afc-4e08-a8d8-a55686753edc" />

- Encrypting the message using command gpg --encrypt --recipient "Niroj" --armor Niroj.txt
<img width="957" height="805" alt="image" src="https://github.com/user-attachments/assets/9869ae98-1f8f-402a-84aa-4ba4b0d2d065" />

- Now, reading the file with ls command and here we can see the new txt file of Niroj with .asc with it Niroj.txt.asc which is the encrypted file
<img width="963" height="796" alt="image" src="https://github.com/user-attachments/assets/ba38c7e5-281c-4e3b-aa3a-e300a9a1e8c4" />

- We decrypt this file by using command gpg --decrypt Niroj.txt.asc in the terminal.
- When we use the command our password protection pops up here and we then insert our password to decrypt our file. 

<img width="959" height="803" alt="image" src="https://github.com/user-attachments/assets/e152e16c-3d33-4fb8-8f3e-39beed08f448" />

- after decryption we can observe the message that was encrypted with in the file.

<img width="956" height="810" alt="image" src="https://github.com/user-attachments/assets/2cbcb3ac-14a6-4867-8e91-304e05638be1" />


# Sources 

- Karvinen, T. 2026. Information Security. Available at: https://terokarvinen.com/information-security/ 
- Karvinen, T. 2023. PGP - Send Encrypted and Signed Message - gpg. Available at: https://terokarvinen.com/2023/pgp-encrypt-sign-verify/
- Schneier, B. 2015. Applied Cryptography: Protocols, Algorithms, and Source Code in C. Chapter 1: Foundations. Available at: https://www.oreilly.com/library/view/applied-cryptography-protocols/9781119096726/08_chap01.html#chap01-sec006














 

