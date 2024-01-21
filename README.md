# cyber-encrypt

cyber-encrypt is a TypeScript library that provides functions for encrypting and decrypting JSON data using the PBKDF2 algorithm and AES encryption. It aims to provide a secure and straightforward way to handle sensitive information.


![Cyber-Encrypt](https://github.com/ala-garbaa-pro/cyber-encrypt/assets/79337368/3101afa3-4356-4089-a8b8-33235d73ec99)

#### Installation

```bash
npm install cyber-encrypt
```

#### Usage

##### encryptJSON

```typescript
import { encryptJSON } from 'cyber-encrypt';

const jsonData = {
  username: 'john_doe',
  password: 'secure_password123',
};

const encryptedData = encryptJSON(jsonData);
console.log('Encrypted Data:', encryptedData);
```

##### decryptJSON

```typescript
import { decryptJSON } from 'cyber-encrypt';

const encryptedData = '...'; // Replace with the actual encrypted data
const decryptedData = decryptJSON(encryptedData);
console.log('Decrypted Data:', decryptedData);
```

#### Configuration

In the `core/config.ts` file, you can customize the encryption parameters such as key size, iterations, and special character escape sequences.

#### File Structure

- **core/config.ts:** Contains configuration parameters for encryption.
- **json/decryptJSON.ts:** Provides a function to decrypt JSON data.
- **json/encryptJSON.ts:** Provides a function to encrypt JSON data.
- **text/decryptText.ts:** Provides a function to decrypt text.
- **text/encryptText.ts:** Provides a function to encrypt text.

#### Important Note

Ensure that you keep your encryption passphrase (`ENV_CYBER_ENCRYPT_PASS_KEY`) secure and do not expose it in public repositories.

#### Contributing

Feel free to contribute by submitting bug reports, feature requests, or pull requests. We welcome your feedback and involvement!

#### License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.

