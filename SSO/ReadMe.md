# SAML security testing 

| Test Case | Attack Vectors |
|-|-|  
| Validate Message Confidentiality and Integrity | - Eavesdropping (7.1.1.1)<br>- Theft of User Authentication Information (7.1.1.2)<br>- Theft of the Bearer Token (7.1.1.3)<br>- Message Deletion (7.1.1.6)<br>- Message Modification (7.1.1.7)<br>- Man-in-the-middle (7.1.1.8)<br>- XML Signature Wrapping |
| Validate Signatures | - Man-in-the-middle (6.4.2)<br>- Forged Assertion (6.4.3)<br>- Message Modification (7.1.1.7)<br>- XML Signature Wrapping<br>- Use of Weak Hashing Algorithms |
| Validate Protocol Usage | - Stolen Assertion (6.4.1)<br>- Man-in-the-middle (6.4.2)<br>- Forged Assertion (6.4.3)<br>- Browser State Exposure (6.4.4)<br>- Replay Attack |  
| Validate Protocol Processing Rules | - Man-in-the-middle (6.4.2)<br>- Stolen Assertion (6.4.1)<br>- Forged Assertion (6.4.3)<br>- Browser State Exposure (6.4.4)<br>- XML Bomb |
| Validate Binding Implementation | - Stolen Assertion (6.4.1)<br>- Replay (6.4.5)<br>- SAML Request/Response Tampering |
| Validate Security Countermeasures | - Stolen Assertion (6.4.1)<br>- Man-in-the-middle (6.4.2)<br>- Browser State Exposure (6.4.4)<br>- Weak Ciphers |
| Unsolicited Response Considerations (SP) | - Replay (6.1.2)<br>- Message Insertion (6.1.3)<br>- Open Redirect<br>- HTTP Response Splitting |  
| Identity Provider (IdP) Considerations | - Validate X.509 Certificate compatibility<br>- Strong Authentication options<br>- IDP validation<br>- Use/Trust Root CAs<br>- Synchronize to common Internet timesource<br>- Define levels of assurance<br>- Prefer asymmetric identifiers<br>- Sign each individual Assertion<br>- Validate Signatures<br>- Validate IDP certificates<br>- Validate NotBefore and NotOnorAfter<br>- Validate Recipient attribute<br>- Define criteria for SAML logout<br>- Exchange assertions over secure transports<br>- Define criteria for session management<br>- Verify user identities obtained from SAML ticket assertions |
| Service Provider (SP) Considerations | - Validating session state<br>- Authorization context granularity<br>- Sign each individual Assertion<br>- Validate Signatures<br>- Validate IDP signatures<br>- Validate IDP certificates<br>- Validate NotBefore and NotOnorAfter<br>- Validate Recipient attribute<br>- Define criteria for SAML logout<br>- Exchange assertions over secure transports<br>- Define criteria for session management<br>- Verify user identities obtained from SAML ticket assertions |
