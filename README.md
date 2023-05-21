# @tripathirajan/crypto-service

Cryptography utility build on the top of bcrypt and crypto for NodeJs.

## Installation

```
npm install @tripathirajan/crypto-service
```

## Usage

```javascript
const { Hashing } = require('@tripathirajan/crypto-service');
Hashing.getHash('payload', 6); // 2nd param is salt length and by default it is 5
```

## Methods

- `getHash(payload, salt=5)`
- `base64Encode(text)`
- `base64Decode(payload)`
- `compareHash(text, hash)`
