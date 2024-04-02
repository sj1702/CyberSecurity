Encryption Overview
Almost every action we take in our modern digital world involves cryptography. Encryption protects our personal and business transactions; digitally signed software updates verify their creator’s or supplier’s claim to authenticity. Digitally signed contracts, binding on all parties, are routinely exchanged via email without fear of being repudiated later by the sender. 

Cryptography is used to protect information by keeping its meaning or content secret and making it unintelligible to someone who does not have a way to decrypt (unlock) that protected information. The objective of every encryption system is to transform an original set of data, called the plaintext, into an otherwise unintelligible encrypted form, called the ciphertext. 

Properly used, singly or in combination, cryptographic solutions provide a range of services that can help achieve required systems security postures in many ways: 

Confidentiality: Cryptography provides confidentiality by hiding or obscuring a message so that it cannot be understood by anyone except the intended recipient. Confidentiality keeps information secret from those who are not authorized to have it. 
Integrity: hash functions and digital signatures can provide integrity services that allow a recipient to verify that a message has not been altered by malice or error. These include simple message integrity controls. Any changes, deliberate or accidental, will result in the two results (by sender and by recipient) being different. 

An encryption system is the set of hardware, software, algorithms, control parameters and operational methods that provide a set of encryption services.

Plaintext is the data or message in its normal, unencrypted form and format. Its meaning or value to an end user (a person or a process) is immediately available for use.

Plaintext can be:

image, audio or video files in their raw or compressed forms
human-readable text and numeric data, with or without markup language elements for formatting and metadata
database files or records and fields within a database
or anything else that can be represented in digital form for computer processing, transmission and storage
It is important to remember that plaintext can be anything—much of which is not readable to humans in the first place.



Symmetric Encryption
The central characteristic of a symmetric algorithm is that it uses the same key in both the encryption and the decryption processes. It could be said that the decryption process is just a mirror image of the encryption process. This image displays how symmetric algorithms work.

The same key is used for both the encryption and decryption processes. This means that the two parties communicating need to share knowledge of the same key. This type of algorithm protects data, as a person who does not have the correct key would not be able to read the encrypted message. Because the key is shared, however, this can lead to several other challenges:

If two parties suspect a specific communication path between them is compromised, they obviously can't share key material along that path. Someone who has compromised communications between the parties would also intercept the key.
Distribution of the key is difficult, because the key cannot be sent in the same channel as the encrypted message, or the man-in-the-middle (MITM) would have access to the key. Sending the key through a different channel (band) than the encrypted message is called out-of-band key distribution. Examples of out-of-band key distribution would include sending the key via courier, fax or phone.
Any party with knowledge of the key can access (and therefore change) the message.
Each individual or group of people wishing to communicate would need to use a different key for each individual or group they want to connect with. This raises the challenge of scalability — the number of keys needed grows quickly as the number of different users or groups increases. Under this type of symmetric arrangement, an organization of 1,000 employees would need to manage 499,500 keys if every employee wanted to communicate confidentially with every other employee.

Primary uses of symmetric algorithms:

Encrypting bulk data (backups, hard drives, portable media)
Encrypting messages traversing communications channels (IPsec, TLS)
Streaming large-scale, time-sensitive data (audio/video materials, gaming, etc.)
Other names for symmetric algorithms, which you may encounter, include:

Same key
Single key
Shared key
Secret key
Session key
An example of symmetric encryption is a substitution cipher, which involves the simple process of substituting letters for other letters, or more appropriately, substituting bits for other bits, based upon a cryptovariable. These ciphers involve replacing each letter of the plaintext with another that may be further down the alphabet.



Asymmetric Encryption
Asymmetric encryption uses one key to encrypt and a different key to decrypt the input plaintext. This is in stark contrast to symmetric encryption, which uses the same key to encrypt and decrypt. For most security professionals, the math of asymmetric encryption can be left to the cryptanalysts and cryptographers to know.

A user wishing to communicate using an asymmetric algorithm would first generate a key pair. To ensure the strength of the key generation process, this is usually done by the cryptographic application or the public key infrastructure (PKI) implementation without user involvement. One half of the key pair is kept secret; only the key holder knows that key. This is why it is called the private key. The other half of the key pair can be given freely to anyone who wants a copy. In many companies, it may be available through the corporate website or access to a key server. Therefore, this second half of the key pair is referred to as the public key.

Note that anyone can encrypt something using the recipient’s public key, but only the recipient —with their private key—can decrypt it.

Asymmetric key cryptography solves the problem of key distribution by allowing a message to be sent across an untrusted medium in a secure manner without the overhead of prior key exchange or key material distribution. It also allows for several other features not readily available in symmetric cryptography, such as the non-repudiation of origin and delivery, access control and data integrity.

Asymmetric key cryptography also solves the problem of scalability. It does scale well as numbers increase, as each party only requires a key pair, the private and public keys. An organization with 100,000 employees would only need a total of 200,000 keys (one private and one public for each employee). This is less than half of the number of keys that would be required for symmetric encryption.

The problem, however, has been that asymmetric cryptography is extremely slow compared with its symmetric counterpart. Asymmetric cryptography is impractical for everyday use in encrypting large amounts of data or for frequent transactions where speed is required. This is because asymmetric key cryptography is handling much larger keys and is mathematically intensive, thereby reducing the speed significantly.

Let’s look at an example that illustrates the use of asymmetric cryptography to achieve different security attributes.

The two keys (private and public) are a key pair; they must be used together. This means that any message that is encrypted with a public key can only be decrypted with the corresponding other half of the key pair, the private key. Similarly, signing a message with a sender’s private key can only be verified by the recipient decrypting its signature with the sender’s public key. Therefore, as long as the key holder keeps the private key secure, there exists a method of transmitting a message confidentially. The sender would encrypt the message with the public key of the receiver. Only the receiver with the private key would be able to open or read the message, providing confidentiality.




Narrator: Examples of encryption persist throughout human history, from early cryptic depictions by cave dwellers of Magura Cave in Bulgaria to the Pyramids at Giza. Even then, each group had its own primitive cryptographic approach, so that members of the tribe or group could communicate with one another while keeping secrets from the rival tribes regarding hunting grounds or sources of water and food.   It is part of human nature to encrypt information. You start with clear text, which is the information that you and I could easily read, and then you use an algorithm, which is often a form of software that can be embedded in the system. But that needs to be activated with an encryption key. A very simple example is if you are trying to encrypt a PDF document; for example, perhaps your accountant is sending you some documents to sign before submitting your taxes. Encryption would create a ciphertext, which no one can use, and you and your accountant would have set up a preset encryption key so that you could retrieve the information at either end of the communication. You need to have good key management, which means you safeguard the information, because imagine if you have thousands of keys in a commercial environment. There is often a third party or external server where the keys will be separately stored and managed, so you don’t have all your eggs in one basket, so to speak. It will be protected through a hashing system, which we will explore in a moment, and no one else can have access to those keys.  Asymmetric encryption is more secure because the sender and receiver each uses a unique code, often a certificate, so you can confirm that the information has been sent from the sender to the recipient in a secure manner.  


Hashing
Hashing takes an input set of data (of almost arbitrary size) and returns a fixed-length result called the hash value. A hash function is the algorithm used to perform this transformation. When used with cryptographically strong hash algorithms, this is the most common method of ensuring message integrity today.

Hashes have many uses in computing and security, one of which is to create a message digest by applying such a hash function to the plaintext body of a message. 

To be useful and secure, a cryptographic hash function must demonstrate five main properties: 

Useful: It is easy to compute the hash value for any given message.
Nonreversible: It is computationally infeasible to reverse the hash process or otherwise derive the original plaintext of a message from its hash value (unlike an encryption process, for which there must be a corresponding decryption process).
Content integrity assurance: It is computationally infeasible to modify a message such that re-applying the hash function will produce the original hash value. 
Unique: It is computationally infeasible to find two or more different, sensible messages that hash to the same value.
Deterministic: The same input will always generate the same hash, when using the same hashing algorithm.

Cryptographic hash functions have many applications in information security, including digital signatures, message authentication codes and other forms of authentication. They can also be used for fingerprinting, to detect duplicate data or uniquely identify files, and as checksums to detect accidental data corruption. The operation of a hashing algorithm is demonstrated in this image.

This is an example of a simple hashing function. The originator wants to send a message to the receiver and ensure that the message is not altered by noise or lost packets as it is transmitted. The originator runs the message through a hashing algorithm that generates a hash, or a digest of the message. The digest is appended to the message and sent together with the message to the recipient. Once the message is delivered, the receiver will generate their own digest of the received message (using the same hashing algorithm). The digest of the received message is compared with the digest sent by the originator. If the digests are the same, the received message is the same as the sent message.

The problem with a simple hash function like this is that it does not protect against a malicious attacker that would be able to change both the message and the hash/digest by intercepting it in transit. The general idea of a cryptographic hash function can be summarized with the following formula:

 
variable data input + hashing algorithm

= fixed bit size data output (the digest)

Even the slightest change in the input message results in a completely different hash value.

Hash functions are very sensitive to any changes in the message. Because the size of the hash digest does not vary according to the size of the message, a person cannot tell the size of the message based on the digest.



Hashing Deep Dive
Hashing puts data through a hash function or algorithm to create an alphanumeric set of figures, or a digest, that means nothing to people who might view it. No matter how long the input is, the hash digest will be the same number of characters. Any minor change in the input, a misspelling, or upper case or lower case, will create a completely different hash digest. So you can use the hash digest to confirm that the input exactly matches what is expected or required, for instance, a password.

For example, we pay our rent through automatic withdrawal, and it’s $5,000 a month. Perhaps someone at the bank or at the rental office thinks they can just change it to $50,000 and keep the extra money. They think no one will notice if they just add another zero to the number. However, that change will completely change the digest. Since the digest is different, it will indicate that someone corrupted the information by changing the value of the automatic withdrawal, and it will not go through. Hashing is an extra layer of defense.

Before we go live with a software product provided by a third party, for instance, we have to make sure no one has changed anything since it was tested by you and the programmer. They will usually send you the digest of their code and you compare that to the original. This is also known as a Checksum. If you see a discrepancy, that means something has changed. Then the security coders will compare the original one and the new one, and sometimes it’s very tedious, but they have software that can do it for them. If it’s something a little more intricate, they may need to go line by line and find out where the bugs are or if some lines need to be fixed. Often these problems are not intentional; they sneak in when you are making final adjustments to the software.

An incident occurred at the University of Florida many years ago, where a very reputable software source, Windows 2000 or Millennium, was provided to 50,000 students via CD-ROMs, and the copies were compromised. The problems were detected when the digests did not match on a distribution file.