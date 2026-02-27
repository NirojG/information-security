# h6 February2026!

## x) One-Way Functions
- One-way functions are easy to compute in one direction but it is significantly harder to reverse.
- So, harder meaning for example if x is given and it is easy to compute from x to f(x) but it would take millions of years to compute f(x) to x even using all the world's computers. so, basically it means it is almost impossible to reverse the function.
- Smashing a plate is a example of a one-way function meaning it is easy to break a plate but its insanely difficult to put it all back to its original form.
- One-wau function cannot be used for encryption because it could never be decrypted. 
- A trapdoor one-way function is a version that includes a hidden secret key, so it is very hard to reverse unless you possess a specific secret key.
- With the secret trapdoor information, the reverse computation becomes easy.

## One-way Hash Functions 
- One-way Hash functions are the building block for many protocols such as compression function, contraction function, message digest, fingerprint, cryptographic checksum, message integrity check (MIC), and manipulation detection code (MDC).
- Hash functions are used in computers from a very long time.
- A hash function which is a function which takes a variable-length input string and converts it to a fixed-length output string called hash value.
- The point is to fingerprint the pre-image to produce a value that indicates if a candidate is likely the same.
- A one-way hash function is easy to compute the hash value, but hard to generate a pre-image that hashes to it.
- A good one-way hash function is collision-free, making it hard to find two pre-images with the same hash value.
- A message authentication code (MAC) it is also known as data authentication code (DAC) which is a one-way hash function with the addition of a secret key.
- Only someone with the key can verify the hash value of a MAC.

## a) Installing hashcat
- Firstly I updated everything with sudo apt-get update
- Secondly I installed hashcat
<img width="961" height="923" alt="image" src="https://github.com/user-attachments/assets/ccedcc9a-7f7a-4358-bb77-cc7db39753bf" />

- I made new directory for our worked named "hashed"
<img width="959" height="918" alt="image" src="https://github.com/user-attachments/assets/39e1dffa-6240-4946-bc52-f4e3293eb3f7" />

- I installed the rockyou dictionary here on my directory. It is one of the most popular dictionary of the passwords.

<img width="823" height="542" alt="image" src="https://github.com/user-attachments/assets/7e56d839-17a1-4700-b677-3bea7dbe9d4e" />

- I proceeded to extract the file as it was compressed and extracted it 

<img width="864" height="695" alt="image" src="https://github.com/user-attachments/assets/f081dadf-6eb3-4932-917f-49429ff3df3d" />

- After extraction of file i checked the file, and since I saw the txt file which i need for later on purposes and the other compressed file i removed it by rm command.

<img width="833" height="559" alt="image" src="https://github.com/user-attachments/assets/83b39ff6-6d09-4d57-a3a3-52131ed1863b" />

- I checked what kind of passwords are there the first 10 we see and there are 14 million others after it. 

<img width="826" height="544" alt="image" src="https://github.com/user-attachments/assets/309a1f4e-8201-4cd2-8400-fa0a8fb530e0" />

<img width="829" height="535" alt="image" src="https://github.com/user-attachments/assets/72bbab2a-12a7-4b42-a24e-5138a338d3aa" />


- Now Identifying the Hash type and starting to crack the task in hand.

<img width="826" height="537" alt="image" src="https://github.com/user-attachments/assets/b3824947-3ead-4591-ad2a-4996489f7fbe" />

- I used this command to solve it hashcat -m 0 'd595b2086532422bbe654bc07ea030df' rockyou.txt -o solved 

<img width="1283" height="798" alt="image" src="https://github.com/user-attachments/assets/b03c6cdf-532f-412c-b234-65a274cf5cb3" />

<img width="1279" height="807" alt="image" src="https://github.com/user-attachments/assets/921349eb-9098-43cc-beca-59356863d510" />

- I now viewed the password that i cracket i used cat solved

<img width="1284" height="801" alt="image" src="https://github.com/user-attachments/assets/03d8986d-8004-49fb-abfc-d2d3047f4c94" />

- The password I cracked was disobey.





