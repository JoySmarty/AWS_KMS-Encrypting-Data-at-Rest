# 🔐 Encrypting Data at Rest using AWS KMS, S3, and EBS

This repository documents my guided AWS lab on encrypting data at rest using Amazon S3, Amazon EBS, AWS KMS, and AWS CloudTrail.

## 🧭 Overview

In this lab, I explored how to protect sensitive data stored in AWS resources using built-in encryption options. The focus was on both default and customer-managed encryption approaches.


# 🧩 Key Steps

- Reviewed S3 Default Encryption

- Uploaded an object to an S3 bucket.

- Verified default SSE-S3 encryption.

- Created AWS KMS Key (MyKMSKey)

- Configured key administrators and key users.

- Enabled usage logging and audit tracking.

- Encrypted EBS Volume

- Created a new encrypted 1 GiB EBS volume.

- Attached it to an EC2 instance.

- Disabled and Re-enabled KMS Key

- Observed how key status affects data access.

- Analyzed CloudTrail Events

- Reviewed key events (CreateGrant, Decrypt, AttachVolume).

- Enabled Automatic Key Rotation

- Set rotation interval to one year.


# 📊 Architecture Summary

- Amazon S3 → SSE-S3 encryption for uploaded objects

- Amazon EC2 + EBS → Encrypted volume using CMK

- AWS KMS → Custom key management and decryption

- AWS CloudTrail → Logged all encryption/decryption operations


# 🧠 Key Learning Outcomes

- Understand AWS encryption mechanisms and KMS integration.

- Implement encryption and key management for compliance.

- Use CloudTrail for security auditing.

- Appreciate the impact of KMS key states on data availability.


# 🧩 Lab Source: AWS Academy Guided Lab — Encrypting Data at Rest by Using AWS Encryption Options

# 👩🏽‍💻 Completed by: Joy Imarah




This exercise deepened my understanding of how AWS integrates encryption and auditing seamlessly — showing that data security in the cloud is not just a configuration, it’s a shared responsibility.

#AWS #CloudSecurity #DevOps #AWSSecurity #AWSKMS #CloudTrail #DataProtection #Encryption #CloudComputing
