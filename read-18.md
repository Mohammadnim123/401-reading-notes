# Ceasar Cipher

Caesar cipher, also known as Caesar’s cipher, the shift cipher, Caesar’s code or Caesar shift, is one of the simplest and most widely known encryption techniques. It is a type of substitution cipher in which each letter in the plaintext is replaced by a letter some fixed number of positions down the alphabet. For example, with a left shift of 3, D would be replaced by A, E would become B, and so on. The method is named after Julius Caesar, who used it in his private correspondence.

>The encryption step performed by a Caesar cipher is often incorporated as part of more complex schemes, such as the Vigenère cipher, and still has modern application in the ROT13 system. As with all single-alphabet substitution ciphers, the Caesar cipher is easily broken and in modern practice offers essentially no communications security.


**Breaking the cipher:**
Two situations can be considered:
an attacker knows (or guesses) that some sort of simple substitution cipher has been used, but not specifically that it is a Caesar scheme: such as frequency analysis or pattern words.
an attacker knows that a Caesar cipher is in use, but does not know the shift value: One way to do this is to write out a snippet of the ciphertext in a table of all possible shifts known as "completing the plain component".

Hashing : Hashing is a type of cryptography that changes a message into an unreadable string of text for the purpose of verifying the message’s contents, not hiding the message itself.This type of cryptography is most commonly used to protect the transmission of software and large files where the publisher of the files or software offers them for download. The reason for this is that, while it is easy to calculate the hash, it is extremely difficult to find an initial input that will provide an exact match for the desired value.

the most common hashing algorithms are MD5 and SHA-1, however due to these algorithm’s multiple weaknesses, most new applications are transitioning to the SHA-256 algorithm instead of its weaker predecessors.

Symmetric Cryptography : Symmetric Cryptography, likely the most traditional form of cryptography, is also the system with which you are probably most familiar. This type of cryptography uses a single key to encrypt a message and then decrypt that message upon delivery.

Since symmetric cryptography requires that you have a secure channel for delivering the crypto key to the recipient, this type of cryptography is all but useless for transmitting data (after all, if you have a secure way to deliver the key, why not deliver the message in the same manner?) Most modern symmetric cryptography relies on a system known as AES or Advanced Encryption Standards.
Asymmetric Cryptography uses two different keys for encryption and decryption, as opposed to the single key used in symmetric cryptography.

The first key is a public key used to encrypt a message, and the second is a private key which is used to decrypt them. The great part about this system is that only the private key can be used to decrypt encrypted messages sent from a public key.
While this type of cryptography is a bit more complicated, you are likely familiar with a number of its practical applications.
Key Exchange Algorithms