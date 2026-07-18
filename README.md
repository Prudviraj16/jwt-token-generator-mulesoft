# MuleSoft JWT Generator

A MuleSoft application that generates JSON Web Tokens (JWT) by securely retrieving a private key from Azure Key Vault.

## Features

- Retrieve Private Key from Azure Key Vault
- Generate JWT Header
- Generate JWT Payload
- Base64URL Encoding
- RSA SHA-256 Signing
- Return Signed JWT
- Built with Mule 4 and DataWeave 2.0

---

## Architecture

Client

↓

Mule API

↓

Azure Key Vault

↓

Private Key

↓

JWT Generation

↓

Signed JWT Response

---

## Technologies Used

- MuleSoft 4
- DataWeave 2.0
- Java
- Azure Key Vault
- JWT
- RSA SHA256
- Maven

---

## Project Flow

1. Receive HTTP Request
2. Fetch Private Key
3. Create JWT Header
4. Create JWT Payload
5. Base64URL Encode
6. Generate Signature
7. Return JWT

---

## Sample Payload

```json
{
  "iat": 1756850400,
  "exp": 1756854000
}
```

## Sample Response

```text
eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCJ9...
```

## Folder Structure

```
src
 ├── main
 ├── test
 └── resources
```

## Future Improvements

- OAuth2 Support
- JWK Support
- Azure Managed Identity
- JWT Validation Endpoint

## Author

Prudviraj Bandari

MuleSoft Developer
