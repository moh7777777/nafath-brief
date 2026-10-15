ersion: NAFATH-V1
Your track: Cybersecurity

## Overview
The NAFATH-V1 single sign-on platform connects six crucial IT fields to deliver a secure and unified government identity environment. At its foundation, software engineering manages identity through robust authentication layers, while mobile platforms enforce strict device access boundaries. Networking architectures mask and route infrastructure requests dynamically, and data governance frameworks protect citizens' information according to regional legislation. Artificial intelligence adds automated risk scoring to block illegal operations in real time. Ultimately, these integrated subtopics create a unified barrier against modern tactical vectors, directly supporting the core architectural objective of implementing phishing-resistant authentication.


## Software

In the world of modern authentication and API security, two protocols often get mixed up — OAuth 2.0 and OpenID Connect (OIDC). They sound similar, share the same foundation, and even use the same endpoints — but they solve different problems.
OAuth 2.0 is an authorization framework — it’s all about granting access
OpenID Connect is an authentication protocol built on top of OAuth 2.0
OpenID Connect → The security desk checks your ID badge to verify who you are (authentication).
OAuth 2.0 → You use a keycard to open specific rooms you’re authorized to access (authorization).
OAuth 2.0 vs OpenID Connect — The Real Difference Explained  https://www.linkedin.com/pulse/oauth-20-vs-openid-connect-real-difference-explained-pandian-aspqc
https://www.oloid.com/blog/oidc-vs-oauth


## AI

Before going live, the authority must manage socio-technical risks outlined in the NIST AI Risk Management Framework 1.0. Key characteristics include ensuring the system is valid and reliable to minimize false positives, secure and resilient against adversarial extraction attacks, and fair with managed bias to prevent discriminatory transaction flagging.
Resource: NIST Artificial Intelligence Risk Management Framework (AI RMF 1.0) - https://nist.gov  https://www.paloaltonetworks.com/cyberpedia/ai-risks-and-benefits-in-cybersecurity

## Mobile
Android’s runtime permission model forces the application to request sensitive permissions dynamically at runtime instead of installation. The application must request access when it explicitly needs to utilize a protected API resource, like biometric hardware or camera streams.
Resource: Android Developers Guide: Request app permissions - https://android.com    https://academy.hsoub.com/programming/android

## Networking
DNS over HTTPS (DoH) encrypts domain name lookups using standard HTTPS sessions. It protects citizens by preventing network eavesdroppers from viewing or altering their DNS queries, but it does not conceal the target server's IP address or the data payloads.
Resource: RFC 8484 - DNS Queries over HTTPS (DoH) - https://rfc-editor.org  https://heimdalsecurity.com/blog/dns-over-https-doh/

## Cybersecurity
An authentication method is phishing-resistant if it cryptographically binds the credential to the specific origin domain of the relying service, preventing interception by proxy websites. Multi-factor methods that utilize FIDO2/WebAuthn hardware keys or cryptographic passkeys qualify. Conversely, legacy multi-factor methods such as SMS-based one-time passwords, mobile push notifications, and standard authenticator app time-based tokens are vulnerable to intercepting proxies and do not qualify.
Resource: NIST Special Publication 800-63B: Digital Identity Guidelines - https://nist.gov         https://www.ibm.com/think/topics/phishing-resistant-mfa

## Data

Under Oman's Personal Data Protection Law (Royal Decree 6/2022), the authority must obtain explicit written consent before data processing, appoint a dedicated data protection officer, report data breaches within 72 hours, and delete citizen records immediately after processing concludes.
Resource: Royal Decree 6/2022 Issuing the Personal Data Protection Law - https://decree.om      https://qanoon.om/p/2022/rd2022006/

## Misconception in My Track

## Misconception in My Track
A common misconception regarding DNS over HTTPS is that transport channel encryption automatically ensures absolute data authentication and verification. In reality, encryption only secures the transit link between the client and the resolver. Section 1.4.9 of the primary specification text proves that transport layer security remains entirely independent from DNSSEC verification. Falsified records or compromised upstream sources will still deliver malicious answers straight through an encrypted tunnel unless cryptographic signature validation is explicitly enforced.

he specific notion that "simply having multi-factor authentication (MFA) of any kind equates to complete protection against compromise" is a misconception

## Open Question
What explicit configuration protocols will the authority implement to securely bootstrap the initial connection to the designated DoH server without creating plain-text lookup loops?
Can the Authority not allow numbers to be withdrawn from users after their expiration date?
How to detect malicious links even when they appear legitimate
