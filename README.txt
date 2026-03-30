About Fastdes: 
We implemented a smaller version of a traditional the Data Encryption Standard  (DES). In our version we used 8 rounds instead of 16 rounds. We also removed initial and final premutation. Through our research we discovered that the premutations do not add much security and it slows down the encryption/decryption process. We used the Feistel network that traditional DES uses so our program has the same structure for encryption and decryption. We also used 4 S-boxes instead of 8. Each of our S-Boxes takes in an 8-bit input and gives out a 8-bit output. This makes our cypher simpiler. We also removed the expention step of F function which made the code more simple and faster. 

to compile: gcc -O2 -o des des.c

to run: ./des

it will prompt for either e for encryption or d for decryption. You will need to provide a key in hex up to 16 digits and if you are encrypting you are able to provide hex plain text of any length. If you are decryption you provide the cyphertext. 
If the plain text provided is not a multiple of 16 the program will pad the left of the plain text with 0s until it is a multiple of 16.