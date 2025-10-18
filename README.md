# 🔐 Encrypting Data at Rest using AWS KMS, S3, and EBS

This repository documents my guided AWS lab on encrypting data at rest using Amazon S3, Amazon EBS, AWS KMS, and AWS CloudTrail.

## 🧭 Overview

In this lab, I explored how to protect sensitive data stored in AWS resources using built-in encryption options. The focus was on both default and customer-managed encryption approaches.


# 🧩 Key Steps

- Reviewed S3 Default Encryption
<img width="1038" height="237" alt="kms1" src="https://github.com/user-attachments/assets/362abc27-3a94-46e2-b196-7f12dde9dec9" />


- Uploaded an object to an S3 bucket.
<img width="1364" height="521" alt="kms2" src="https://github.com/user-attachments/assets/5ef70bbe-e327-496b-a2a8-8ee260838b9b" />

- Verified default SSE-S3 encryption.

- Created AWS KMS Key (MyKMSKey)
<img width="1365" height="406" alt="kms3" src="https://github.com/user-attachments/assets/329f9708-fb97-4675-8af5-8570715c5316" />

- Configured key administrators and key users.

- Enabled usage logging and audit tracking.

- Encrypted EBS Volume

- Created a new encrypted 1 GiB EBS volume.
<img width="1357" height="584" alt="kms6" src="https://github.com/user-attachments/assets/e122eb1a-e6aa-4545-80fa-0dd496edf75c" />

- Attached it to an EC2 instance.
<img width="1348" height="570" alt="kms7" src="https://github.com/user-attachments/assets/fa65a17a-ddda-497e-8998-4375a3726412" />
<img width="1330" height="528" alt="kms8" src="https://github.com/user-attachments/assets/f2835bfe-a290-4ced-8176-5a131f4f74b0" />
<img width="1059" height="167" alt="kms9" src="https://github.com/user-attachments/assets/06fa8a08-171e-4b7c-ad61-3a910f064ae3" />

- Disabled and Re-enabled KMS Key
<img width="1067" height="306" alt="kms10_" src="https://github.com/user-attachments/assets/e81f9c7e-18bb-4449-94d8-a59807056a00" />
<img width="1088" height="294" alt="kms13" src="https://github.com/user-attachments/assets/e821ec81-7a88-4031-9388-cae15b96e838" />

- Observed how key status affects data access.
<img width="1360" height="552" alt="kms10" src="https://github.com/user-attachments/assets/80451840-922f-4119-b509-a7a3663722ed" />

- Analyzed CloudTrail Events
<img width="1363" height="591" alt="kms12" src="https://github.com/user-attachments/assets/bd25b594-0a9e-478f-9645-f1d75cb75744" />

- Reviewed key events (CreateGrant, Decrypt, AttachVolume).
<img width="1344" height="533" alt="kms11" src="https://github.com/user-attachments/assets/c311bd45-8d70-4dfd-8e94-f4f76584976b" />
<img width="1127" height="316" alt="kms14" src="https://github.com/user-attachments/assets/3ccdb970-1cbd-4a41-934b-a7aebbb88679" />

- Enabled Automatic Key Rotation
<img width="1032" height="217" alt="kms15" src="https://github.com/user-attachments/assets/bc5d5634-752e-4f50-a03a-261e21ca8a39" />

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
