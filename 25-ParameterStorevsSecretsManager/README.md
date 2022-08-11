# Parameter Store (Component of AWS Systems Manager SSM)

* Secure serverless storage for configuration and secrets.
* Passwords
* Database connection strings

- Values can be stored encrypted KMS or plaintext

- Set TTL to expire values such as passwords

- No cost to use, however there is a limit of 10,000 parameters per account


# Secrets Manager (SSM)
- 10K+
- Automatically rotate secrets
- Charged per secret stored and per 10k API calls
- Apply the newkey/password in RDS for you
- Generate random secrets
- Very useful for Cloud Formation