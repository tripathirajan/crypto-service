# @tripathirajan/crypto-service

Cryptography utility build on the top of bcrypt and crypto for NodeJs.

## Installation

```
npm install @tripathirajan/crypto-service
```

## Usage

Add `SECRET_KEY` in your .env file

```javascript
const { Hashing, CryptoAgent } = require('@tripathirajan/crypto-service');
Hashing.getHash('payload', 6); // 2nd param is salt length and by default it is 5
```

## Methods

### Hashing

- `getHash(payload, salt=5)`
- `base64Encode(text)`
- `base64Decode(payload)`
- `compareHash(text, hash)`

### CryptoAgent

- `encrypt(text, key)`
- `decrypt(text, key)`
