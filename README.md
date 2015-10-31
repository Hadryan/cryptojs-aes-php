URL Friendly encryption/decryption by both Javascript and PHP (Same results)
Ideal for: Client side encryption and server side decryption or vice versa

Based on:
CryptoJS 3.x AES encryption/decryption on client side with Javascript and on server side with PHP
================

I've long researched to make this working for me and i want to share my solution to make it possible to encrypt/decrypt data from/to CryptoJS and PHP.
This works with CryptoJS 3.x and PHP with openssl support.

I use a JSON format for encryption/decryption to be able to use any possible object/array/string data on both sides.
I also use the standard AES implementation from CryptoJS with a passphrase. I don't generate special keys, iv's or salts.

Requirements
====
* PHP 5.4+ or higher
* PHP with OpenSSL Support: http://php.net/manual/en/openssl.installation.php
