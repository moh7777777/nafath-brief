ersion: NAFATH-V1
Your track: Cybersecurity

## Overview
markdown
The NAFATH-V1 project establishes a secure, single sign-on national digital identity platform linking multiple public platforms via web and mobile interfaces. High-security software protocols authenticate identity and manage access delegation across systems, while an underlying artificial intelligence model continuously flags unauthorized account access. Mobile operating system constraints dictate strict client-side data boundaries, as networking protocols protect citizen connection integrity against eavesdropping. Operations remain fully bound by national data protection frameworks, which mandate rigorous governance when processing citizen metrics. Because credential interception undermines national trust, the cornerstone of this entire infrastructure is deployment of phishing-resistant authentication methods.
## Software
OAuth 2.0 is an authorization framework designed for delegated access to resources via scoped tokens, but it does not inherently verify user identity. OpenID Connect is an authentication layer built directly on top of OAuth 2.0 that introduces an ID token to securely handle user login.
Resource: Final: OpenID Connect Core 1.0 incorporating errata set 2 - https://openid.net
## AI
Before going live, the authority must manage socio-technical risks outlined in the NIST AI Risk Management Framework 1.0. Key characteristics include ensuring the system is valid and reliable to minimize false positives, secure and resilient against adversarial extraction attacks, and fair with managed bias to prevent discriminatory transaction flagging.
Resource: NIST Artificial Intelligence Risk Management Framework (AI RMF 1.0) - https://nist.gov

## Mobile
Android’s runtime permission model forces the application to request sensitive permissions dynamically at runtime instead of installation. The application must request access when it explicitly needs to utilize a protected API resource, like biometric hardware or camera streams.
Resource: Android Developers Guide: Request app permissions - https://android.com
## Networking
DNS over HTTPS (DoH) encrypts domain name lookups using standard HTTPS sessions. It protects citizens by preventing network eavesdroppers from viewing or altering their DNS queries, but it does not conceal the target server's IP address or the data payloads.
Resource: RFC 8484 - DNS Queries over HTTPS (DoH) - https://rfc-editor.org
## Cybersecurity
An authentication method is phishing-resistant if it cryptographically binds the credential to the specific origin domain of the relying service, preventing interception by proxy websites. Multi-factor methods that utilize FIDO2/WebAuthn hardware keys or cryptographic passkeys qualify. Conversely, legacy multi-factor methods such as SMS-based one-time passwords, mobile push notifications, and standard authenticator app time-based tokens are vulnerable to intercepting proxies and do not qualify.
Resource: NIST Special Publication 800-63B: Digital Identity Guidelines - https://nist.gov

## Data

Under Oman's Personal Data Protection Law (Royal Decree 6/2022), the authority must obtain explicit written consent before data processing, appoint a dedicated data protection officer, report data breaches within 72 hours, and delete citizen records immediately after processing concludes.
Resource: Royal Decree 6/2022 Issuing the Personal Data Protection Law - https://decree.om
## Misconception in My Track


## Open Question
