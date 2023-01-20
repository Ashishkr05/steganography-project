# Design and Implementation of securing data using Cryptography and Steganography
<p>It is  a Python based application with use of flask a microservice based
framework to demonstrate the combination of cryptography that is based on symmetric key and
steganography that is based on modified LSB which helps to provide security to confidential data over
an unsecured network.</p>

# Project Team Members :
<ul>
<li><b>Ashish kumar (201901275) </b></li>
<li><b>Kunj Modi (201901036) </b></li>
<li><b>Tejot Dev (201901149) </b></li>
<li><b>Nirav Damor (201901156) </b></li>
</ul>

<br>


# METHODOLOGY : 
<div>
<p>
  First, we take the original data and encrypt it into
ciphertext by utilizing the proposed symmetric cryptography method in which we will break the 128 bits
into 4 equal groups of 32 bit each this 32-bit block will be undergone some circular shift and xor
operations with secret keys . ( These ideas are inspired by [1] and [2] ). After this, the encrypted data will
be embedded in a Cover Image by use of proposed steganography strategy which is utilizing least
significant bit (LSB) [ In this we are think of going with a mixture of LSB-1, LSB-2, LSB-3 (i.e storing at
first, second, and a third bit from the least significant side) alternatingly. ] to finally create a new image
which is a stego content this is sent over the channel and at receiver side the same process will occur
but in reverse, starting from extracting encrypted content from stego and finally decrypting using
proposed decryption algorithm again inspired by [1] and [2]. Although ideas are inspired, we will use our
own proposed architecture for encryption and decryption finally converting into an application for
sending data over insecure channels.
</p>
</div>



