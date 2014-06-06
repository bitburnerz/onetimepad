#One Time Pad

#General Usage
A series of random numbers is shared between two parties and exchanged in person or over a secure channel. It is the secret key common to both parties. One copy is used for encryption while the other for decryption.

When communicating over an unsecure channel, in order to send a message, the first person would perform encryption by *adding* the value of the plain text message to the value of the shared key. This produces the cipher text. On the receiving end, to perform decryption, the cipher text received is *substracted* by the the value of the shared key. This reproduces the original plain text message.

#Complementary Pads

Because substraction is tedious and for sake of simplicity, what would be greatly helpful is if *both* parties would simply use addition.

Typically, the two copies of the shared secret key are identical. One is used for encryption by addition, and the other for decryption by substraction.

In order to enable us to perform addition on *both* ends and come up with the same result, then another factor needs to change, and this will be the composition of the secret key. Instead on the two copies being identical on both ends, they will now be different, but complementary.

#Using digits over letters
It is quicker and easier to encrypt and decrypt by hand i


This implementation of the One Time Pad allows to:

 - use a set of random numbers to generate a matching encryption and decryption pad with proper formatting, pad numbering, etc.
 - 

Encrypting

To encrypt one must first convert the plain text characters to decimal numbers. The use of regular numbers allows for easy encrypting and decrypting in the field.



To do this we convert every character in the plain text field box to its UTF-8in decimal form. With UTF-8 encoding, one character may take anywhere from 1 to 4 bytes. Every byte will be represented by three decimal digits
