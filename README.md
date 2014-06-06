#One Time Pad

##Philosophy

###General Usage
A series of random numbers is used as a shared secret key between two parties; one for encryption and one for decryption.

These random numbers can either be letters or actual numbers. In the end the principle is the same, only that conversions/tables would be needed required to convert from one to the other.


Typically to encrypt one would add the numerical value of the plain text to the numeric value of the key and send off the resulting encrypted value. (PLAIN + KEY = ENCRYPTED) On the other end, to decrypt the message, the numerical value of the encrypted text is *substracted* with the value of the Key. (ENCRYPTED - KEY = DECRYPTED)

###One Time Pad Improved

For sake of simplicity, consistency, and ease of calculation, two

1- 



###Using digits over letters
It is quicker and easier to encrypt and decrypt by hand i


This implementation of the One Time Pad allows to:

 - use a set of random numbers to generate a matching encryption and decryption pad with proper formatting, pad numbering, etc.
 - 

Encrypting

To encrypt one must first convert the plain text characters to decimal numbers. The use of regular numbers allows for easy encrypting and decrypting in the field.



To do this we convert every character in the plain text field box to its UTF-8in decimal form. With UTF-8 encoding, one character may take anywhere from 1 to 4 bytes. Every byte will be represented by three decimal digits
