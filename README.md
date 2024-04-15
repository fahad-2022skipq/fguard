# fguard
fguard is a powerful npm package for securely encrypting and decrypting sensitive passwords in your Node.js applications. Utilizing advanced cryptographic techniques, fguard ensures that your passwords remain protected from unauthorized access.
## How to install

To install this package, you can use the following npm command:

```bash
npm i fguard
```
## How to use
You can use this package to encrypt and decrypt messages securely.

### Using ES Modules
```bash
import { encrypt, decrypt } from 'fguard';
```
### Using CommonJS
```bash
const { encrypt, decrypt } = require('fguard');
```
In the encrypt function, pass your message as the first argument and the encryption key as the second argument. 
```bash
const message = 'Hello, world!';
const key = 'my-secret-key';

const encryptedMessage = encrypt(message, key);
console.log('Encrypted:', encryptedMessage);
```
The decrypt function takes the encrypted message as the first argument and the same key used for encryption as the second argument.
```bash
const decryptedMessage = decrypt(encryptedMessage, key);
console.log('Decrypted:', decryptedMessage);
```
