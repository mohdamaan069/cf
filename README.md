# OpenSSL Commands for Certificate and Key Management

This repository contains OpenSSL commands for various tasks related to RSA keys, Certificate Signing Requests (CSRs), and certificates.

## 1. Generate RSA Private Key

This command generates a 2048-bit RSA private key and saves it to a file named `private.key`:

```bash
openssl genrsa -out private.key 2048

## 2. Generate CSR (Certificate Signing Request)

This command generates a new RSA private key and CSR. The private key will be saved as `custom.key` and the CSR as `custom.csr`:

```bash
openssl req -nodes -newkey rsa:2048 -keyout custom.key -out custom.csr

