# AWS KMS

- Regional Basis - Keys created in Northern Virginia, can't use in Ohio
- Key Management Service
- Manage Customer Master Keys.
- S3 primarily
- Used to Encrypt and Decrypt
- up to 4KB in size

KMS is on shared hardware with other customers, it is not dedicated or isolated.

# CloudHSM

Does what KMS can do, but more.
- Dedicated Hardware Security Module (HSM)
- FIPS 140-2 Level 3
- Single Tenant, dedicated hardware, multi-AZ cluster
- 2 or 3 in each Region so you can make sure you can decrypt the files

* Certified Security Specialty, and go into a deep dive.
* Security in AWS has a long future.