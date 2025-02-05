# Single Sign-On (SSO) System for St. John’s Clinic

### Overview
This project proposes a Single Sign-On (SSO) system for St. John’s Clinic to enhance the security, confidentiality, and integrity of sensitive patient data.

**Key Features** 
 🔐 **User Registration**:
    - Username and department hashed using SHA-256.
    - Password secured with PBKDF.
    - Data transmitted securely via TLS and stored in an encrypted cloud database.
 🛡️ **SSO Implementation**:
    - OAuth-based authentication with session tokens.
    - Tokens encrypted with AES and transferred securely via TLS.
    - Role-Based Access Control (RBAC) and Two-Factor Authentication (2FA) for enhanced security.
 💾 **Secure Data Storage & Transfer**:
    - Data encrypted using AES and stored in a cloud database.
    - Secure data transfer ensured via TLS.
 🔑 **Cryptographic Protocols**:
    - Hybrid encryption using RSA for key exchange and AES for data encryption.
    - Ensures secure communication and data integrity.
 🔑 **Key Management**:
    - Systematic approach for key generation, exchange, storage, rotation, and retirement.
    - Utilizes Public Key Infrastructure (PKI) for secure key distribution.

### System Workflow
 🔒 **User Authentication**:
  - User logs in with credentials.
  - Credentials validated against hashed data in the database.
  - 2FA (OTP) required for additional security.
 🎟️ **Token Generation**:
  - Session token generated using RNGCryptoServiceProvider.
  - Token encrypted with AES and transmitted via TLS.
 ✅ **Access Granting**:
  - Token decrypted and validated on the server.
  - User granted access to multiple services via OAuth.

### Regulatory Compliance
The system adheres to:
- 📜 GDPR, CCPA, and PSD2 for data protection.
- 🏥 NHS UK guidelines for healthcare data security.

### Common Vulnerabilities & Mitigation
 ⚠️ **Data Tampering**:
  - Mitigated by AES encryption and TLS for secure transfer.
 🔄 **Unpatched Vulnerabilities**:
  - Regular software and hardware updates.
 🔓 **Unauthorised Access**:
  - RBAC and 2FA to restrict access.
 🛑 **Phishing/Social Engineering**:
  - Email filters and user training.

### Conclusion
The SSO system at St. John’s Clinic ensures secure, efficient, and user-friendly access to healthcare services while maintaining data confidentiality, integrity, and availability. By leveraging advanced cryptographic protocols and compliance measures, the system mitigates cyber risks and enhances operational security.
