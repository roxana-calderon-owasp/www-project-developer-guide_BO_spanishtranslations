---

title: Cryptographic Practices
layout: col-document
tags: OWASP Developer Guide
author:
contributors:
document: OWASP Developer Guide
order: 603

---

{% include breadcrumb.html %}
### 6.3 Cryptographic Practices

The OWASP Development Guide is being rewritten by the OWASP community.
and the content of this section has yet to be filled in.

If you would like to contribute then follow the 
[contributing guidelines](https://github.com/OWASP/www-project-developer-guide/blob/main/CONTRIBUTING.md)
and submit your content for review.

The following subsections are planned:

  * Cryptographic Practices
    * Data protection
    * Communication security
    * TLS certificate management
    * Database security
    * Hashes 
    * File hashes, password hashes, salting
    * Verification of hashes for integrity and signature	
    * Secrets handling
    * Keys (generation, lifecycle management), secrets, API keys

Cryptographic practices

* The basis for usage of PKI is to address (using encryption and hashing)
* Confidentiality
* Integrity
* Authentication 
* Non-repudiation
* Cryptography is used for the following:
o Data-at-rest protection using data encrypting keys and key encrypting keys. For which, 
* Do not use custom cryptographic algorithms / deprecated algorithms
* Do not use passwords as cryptographic keys
* Do not hard-code cryptographic keys in the application
* Persist secret keys in a secure vault like HSM, KMS, Secrets Manager
* Manage encryption keys through the lifecycle, including key retirement/replacement when someone who has access leaves the organisation
* Rotate keys on a regular basis. However this depends on the key strength and the algorithm used. If the key strength is low, the rotation period will be smaller
* Maintain a contingency plan to recover data in the event of an encrypted key being lost
* Ensure the code eliminates secrets from memory.
* Maintain a contingency plan that can recover data in the event of an encrypted key being lost
* Store keys away from the data
* Do not use IV twice for a fixed key
o Communication security
* Ensure no sensitive data is transmitted in the clear, internally or externally.
* Validate certificates properly against the hostnames/users for whom they are meant
* Failed TLS connections should not fall back to an insecure connection
* Do not use IV twice for a fixed key
o Cryptography in general
* All protocols and algorithms for authentication and secure communication should be well vetted by the cryptographic community.
* Perform Message integrity checking by using a �combined mode of operation,� or a MAC based on a block cipher.
* Do not use key sizes less than 128 bits or cryptographic hash functions with output sizes less than 160 bits.
* Do not use custom cryptographic algorithms that have not been vetted by cryptography community
* Do not hardcode cryptographic keys in applications?
* Issue keys using a secure means.
* Maintain a key lifecycle for the organisation (Creation, Storage, Distribution and installation, Use, Rotation, Backup, Recovery, Revocation, Suspension, Destruction) 
* Lock and unlock symmetric secret keys securely
* Maintain CRL (Certificate Revocation Lists) maintained on a real-time basis
* Validate certificates properly against the hostnames/users for whom they are meant
* Ensure the code eliminates secrets from memory
* Specific encryption, in addition to SSL
* Mask or remove keys from logs
* Use salted hashes when using MD5 or any such less secure algorithms
* Use known encryption algorithms, do not create your own as they will almost certainly be less secure
* Persist secret keys in a secure vault like HSM, KMS, Secrets Manager
* Do not use IV twice for a fixed key 
* Ensure that cryptographic randomness is used where appropriate, and that it has not been seeded in a predictable way or with low entropy. Most modern APIs do not require the developer to seed the CSPRNG to get security.
	


