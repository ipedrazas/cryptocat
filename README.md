## Cryptocat - browser-based webapp for encrypted chat
### http://crypto.cat
#### Beta software - code review highly appreciated.

Cryptocat lets you instantly set up secure conversations. It's an open source encrypted, private alternative to invasive services such as Facebook chat.

## Cool features
* A client-side 4096-bit Diffie-Hellman-Merkle public key agreement engine.
* A client-side AES-256 implementation is used to encrypt data.
* HMAC message integrity verification.
* The identity of chatters can be confirmed via key fingerprints, à la OTR.
* A seeded, cryptographically secure random number generator that relies on browser elements, DOM, JavaScript variable state, and more to produce entropy. The resulting entropy is hashed to produce the final seed, which is then fed back to the CSPRNG.
* [Cryptocat Verifier](https://chrome.google.com/webstore/detail/dlafegoljmjdfmhgoeojifolidmllaie), a Google Chrome browser extension, can be used to verify the integrity of your Cryptocat session.
* Chats are securely deleted after 30 minutes of inactivity.
* A sleek design with time-stamping, optional audio notifications, fluid-window mode, and mobile support.

## License
### Cryptocat is released under the [Creative Commons Attribution-NonCommercial-ShareAlike 3.0 Unported License](http://creativecommons.org/licenses/by-nc-sa/3.0/):
* Noncommercial — You may not use this work for commercial purposes.
* Attribution — You must attribute the work to the Cryptocat project (but not in any way that suggests that they endorse you or your use of the work).
* Share Alike — If you alter, transform, or build upon this work, you may distribute the resulting work only under the same or similar license to this one.

## Important notes
* Cryptocat provides strongly encrypted, secure communications. However, it is not a replacement to GPG. Think responsibly if you are in extreme, life-threatening situations.

* Paranoid users may want to install [Cryptocat Verifier](https://chrome.google.com/webstore/detail/dlafegoljmjdfmhgoeojifolidmllaie), a Chrome extension that verifies that your Cryptocat session is not serving you modified JavaScript code.

* The code for secure deletion of idle chats after 30 minutes is not included in the Cryptocat git repository. On the [production server](https://crypto.cat), it's actually a cron job that checks the modification time of chats and [wipe](http://linux.die.net/man/1/wipe)s them securely. Those wanting to set up similar functionality should consider writing something similar.

## About
Cryptocat is developed by [Nadim Kobeissi](http://nadim.cc). It uses parts of the [crypto-js](http://code.google.com/p/crypto-js/) library and the Bitcons iconset. Furthermore, Cryptocat is indebted to Paul Brodeur, David Mirza, Hasan Saleh, and Tina Salameh for their helpful suggestions and beta testing.