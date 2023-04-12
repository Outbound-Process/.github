---
name: Fill out ECCN Questionnaire
about: Requestor is asked to fill out the ECCN Questionnaire
title: Fill out ECCN Questionnaire
labels: ["Requestor Action"]
assignees: ''

---

@Requestor: Please fill out this ECCN Questionnaire. After completion, please send an e-mail to [SAP Export Control Classification](mailto:ExportControlClassification@sap.com) with a link to this questionnaire.

# Export Control Classification Questionnaire for Outbound Open Source Contributions

Uploading software to an External Repository as part of the Outbound Open Source process is considered an export. Therefore, export control laws and regulations may apply.  
SAP checks each delivery of software (physical delivery and electronic download) against applicable EU and US export regulations. This process is critical in several cases, for example when cryptographic code is present, implemented, used; or when the software has been developed for customers who are in the defense business or in collaboration with a military organization.
If we have the indication that such cases apply to the planned publication, the export control classification process is mandatory to ensure that export regulations are fulfilled and all data in the determination of export regulations is collected for each open source publication. This process is necessary to ensure SAP does not violate export control regulations.
The violation of export control regulations can result not only in significant fines for SAP but also in criminal penalties for individuals responsible, especially if the submitter of a questionnaire submits incorrect information. Therefore, you should answer the following questions with care and truthfully.
The following questions have to be answered considering all parts of the outbound open source contribution, including re-used SAP components, open source, or third-party components.
If you have further questions, please contact: [SAP Export Control Classification](mailto:ExportControlClassification@sap.com).

## General Data

### Name of the Outbound Open Source Contribution

```
(Provide your answer here)
```

### Language

```
(Provide your answer here)
```

### Used Repository

```
(Provide your answer here)
```

### Release Date

```
(Provide your answer here)
```

### Requestor name and User ID

```
(Provide your answer here)
```

### Date when this questionnaire has been completed

(Do you have a deadline for the intended contribution? Why?)

```
(Provide your answer here)
```

## Export Classification Questions

### 1. Please give a short Functional description of this Product/Component/FOSS. i.e., What is the Product/Component/FOSS designed to do?

```
(Provide your answer here)
```

### 2. Is the primary purpose of this Product/Component/FOSS any of the following items? Check ANY line item that is the primary purpose

- [ ] Information Security (may include products like cryptographic accelerators, key storage, cryptographic libraries)
- [ ] Performing or simulating functions of a digital communication or networking system, equipment, or component (may include products like networking systems/applications, VoIP, communications)
- [ ] Information storage or processing (may include products like databases, operating systems, toolkits, SDKs)
- [ ] NOT APPLICABLE: This PV/CV/FOSS primary functionality is NOT any of the above

If you checked Yes to the first 3 items, please tell why you believe it is the primary purpose.
```
(Provide your answer here)
```

### 3a. How will the Product/Component/FOSS be delivered (Delivery Channel)? Check ALL that apply

- [ ] SWDC/SMP (An S-User # is required to download from SAP’s Software Download Center)
- [ ] Repository-Based Shipment Channel (RBSC)
- [ ] SAP Service Portal
- [ ] Delivered as SOURCE CODE, not compiled

- [ ] Cloud-based (no delivery or download, this is access to SaaS only)

#### MASS MARKET

- [ ] Apple Store
- [ ] Mac Store
- [ ] Google Play
- [ ] Microsoft/Windows Marketplace
- [ ] SAP Store
- [ ] Other Store*

#### PUBLICLY AVAILABLE (SEE URL BOX BELOW TO ADD URL (Required) of this PV/CV/FOSS)

- [ ] Github / GitLab
- [ ] Maven
- [ ] RubyGems
- [ ] PyPI
- [ ] npm
- [ ] Docker Hub
- [ ] Nuget
- [ ] Tools (e.g. tools.hana.ondemand.com)
- [ ] Other Repository*

- [ ] Other* (or indicate which delivery channel you are using)

If "Other Store", "Other Repository" or "Other" was selected above, please describe the delivery method, delivery channel or other relevant information along with a usable URL for that location:
```
(Provide your answer here)
```

### 3b. URL BOX: For publicly available source code, list the URL of the Source Code download location – NO OTHER TEXT, only the URL: (https://...) 

```
(Provide your answer here)
```

## CONSIDER COMPRISED COMPONENTS OR OWN IMPLEMENTATION for this question

### 4. CHECK ALL THAT APPLY:  Does the Product/Component/FOSS USE or IMPLEMENT cryptography for any of the below reasons from its comprised components (called ‘dependencies’ for FOSS) or its own implementation for crypto?

- [ ] **NO encryption** comprised or from its own implementation is included
- [ ] The cryptographic or cryptanalytic functionality is **inactivated** in a way that it cannot be used by the end-user or can only be used with a specific crypto license key or other secure activation method that the end-user needs to acquire separately; (different from encryption not being used)
- [ ] Uses **ONLY** encryption algorithms of **equal to or less than** 56 bits symmetric, equal to or less than 512 bits asymmetric OR equal to or less than 112 bits elliptic curve encryption
- [ ] **Hashing** (e.g., MD5, SHA, SALT) for data integrity – to ensure data is not tampered with
- [ ] **Data confidentiality** – securing data in transit or at rest (e.g., SSL / TLS / HTTPS / AES / 3DES)
- [ ] **Digital Signature / Non-Repudiation** (e.g., docusign, provides proof of origin, guarantee, RSA private key used to sign documents)
- [ ] **Authentication – user credentials** (e.g., name and password, system credentials)
- [ ] **Digital Rights Management** (copyright protection) (e.g., license key product protection, piracy and theft prevention)
- [ ] **Data Integrity Control**
- [ ] OTHER: Fill in text box below
```
(Provide your answer here)
```

If the Product/Component/FOSS is using the comprised components to perform any encryption not noted above, please explain **what** encryption is being performed and **what data** is being encrypted.
```
(Provide your answer here)
```

## ONLY CONSIDER OWN IMPLEMENTATION for this question

### 5.Is this Product/Component/FOSS "crypto-aware" (e.g. makes calls to an underlying structure (platforms, operating systems, etc.) or other software (products, components, FOSS, etc.) to perform cryptography such as SSL/TLS with data encrypted either in transit or encrypted at rest.)

- [ ] No
- [ ] Yes

If Yes, please note **what** functions (e.g. TLS/SSL, etc.) are used and for **what purposes** (stored data, encrypting data in transit, communications, management data, internal data, etc.)
```
(Provide your answer here)
```

### 6. Do any of the following factors about the PV/CV/Foss apply? Check ALL that apply

- [ ] **INSTALLATION:** The Product/Component/FOSS is designed for installation by the user without further substantial support by the supplier (i.e., SAP)
- [ ] **EASILY CHANGEABLE CRYPTO:** The cryptographic functionality is NOT easily changeable by the user
- [ ] **WIDE INTEREST RANGE:** The Product/Component/FOSS is of interest to a wide range of individuals and/or businesses
- [ ] **PRICING:** If being sold, price and information about the main functionality of the product ARE available before purchase without the need to consult SAP of any of SAP’s suppliers
- [ ] None of the above

### 7. Is the PV/CV/FOSS a cryptographic library, development kit or toolkit (SDK) such that an END-USER(S) can MAKE CHOICES about the type of encryption used in the applications or HOW to implement the encryption? Check all that apply

- [ ] **YES, and this is a Cryptographic Library** (e.g. Common Crypto-lib 8, Bouncy Castle, Open SSL, BSAFE)
- [ ] **YES, and this is a Cryptographic Development Kit/Toolkit (SDK)** (e.g. AWS encryption SDK)
- [ ] **NO:** The End Users cannot make choices about the type of encryption used in the applications or HOW to implement the encryption
- [ ] **Not Applicable:** None of the above (No crypto is either included or its own implementation)

If either/both the first and second are checked yes: Explain what this PV/CV/FOSS _is capable_ of doing.
```
(Provide your answer here)
```

### 8. Does this Product/Component/FOSS contain item(s) capable of performing cryptography?

- [ ] No
- [ ] Yes

### 9. It is assumed the software DOES NOT contain or use any of the below. If it does, Check ALL that apply

- [ ] This PV/CV/FOSS contains an **Open Cryptographic Interface (OCI)**
- [ ] This PV/CV/FOSS uses **non-standard encryption algorithm** (proprietary or unpublished cryptography)
- [ ] This PV/CV/FOSS **exposes source code for any encryption functions**
- [ ] None of the above

If you selected one of the first 3 boxes, please explain/describe the OCI, the proprietary/unpublished or non-standard encryption algorithm, the URL of the exposed source code with an explanation in the text box below:
```
(Provide your answer here)
```

### 10. Please check any boxes that are applicable about this Product/Component/FOSS

- [ ] **MILITARY APPLICATION:** has been specially designed, developed, configured or modified for a military application.
- [ ] **INTELLIGENCE APPLICATION:** has been specially designed, developed, configured or modified for an intelligence (Secret Service, not business intelligence) application
- [ ] **INTELLIGENCE OR PUBLIC SECURITY:** has been specially designed, developed, configured or modified for, or with the assistance of, a military, intelligence or public security entity (e.g. as part of a Customer specific development project)
- [ ] **GOVERNMENT END-USE:** modified or customized for government end-user(s) or government end-use (e.g. to secure departmental, police, state security, or emergency response communications)
- [ ] **CUSTOM CUSTOMER SPECIFICATION** the cryptographic functionality has been modified /customized to customer specification
- [ ] **BANKING AND MONEY:** has been specially designed and limited for banking use or money transactions
- [ ] **ANALYSIS AT APPLICATION LAYER:** has been specially designed or modified to perform analysis at the application layer (e.g., Layer 7 of Open Systems Interconnection (OSI) model (ISO/IEC 7498-1)) on a carrier class Internet Protocol (IP) network (e.g., nation grade IP Backbone)
- [ ] **TELECOMMUNICATION DATA RETENTION:** has been specially designed or modified to perform telecommunication data retention (or data preservation) for “intercept Related Information’ (IRI, e.g. ETSI TS 102 656 or similar specifications or standards) within public networks
- [ ] **INTRUSION SOFTWARE:** has been specially designed or modified for the generation, operation or delivery of, or communication with, “intrusion software”
- [ ] **SURREPTITIOUS INTRUSION:** has been designed or modified using mechanical, electrical, or electronic means to detect surreptitious intrusion (Only refers to physical layer security. The physical layer includes Layer 1 of the Reference Model of Open Systems Interconnection (OSI) (ISO/IEC 7498-1))
- [ ] **REDUCE EMANATIONS/SIGNALS:** has been specially designed or modified to reduce the compromising emanations of information bearing signals beyond what is necessary for health, safety, or electromagnetic interference standards
- [ ] **PERFORM CRYPTANALYTIC FUNCTIONS:** has been designed or modified to perform cryptanalytic functions or to develop software or commodities for the development, production or use of cryptanalytic commodities or software
- [ ] **DIGITAL COMPUTERS, ELECTRONIC ASSEMBLIES:** has been specially designed or modified for the “development” or “production” of the following equipment:
  - “Digital computers” having an “Adjusted Peak Performance” (“APP) exceeding 15 Weighted TeraFLOPS (WR); or
  - “Electronic assemblies” specially designed or modified for enhancing performance by aggregation of processors so that the “APP” of the aggregation exceeds the limit of 15 WT.
- [ ] **QUANTUM CRYPTOGRAPHY:**  has been designed or modified to use quantum cryptography
- [ ] **VULNERABIULITY ANALYSIS:**  provides or performs vulnerability analysis, network forensics, or computer forensics functions.
- [ ] **DIRECT PRODUCT** [only applicable to PVs]: the product is a “direct product” of specific technology or software
- [ ] **ENABLES OTHER ITEM:** another item (i.e. another software or hardware) to perform Cryptography or any information security functions (e.g. encryption, decryption, key management/public key infrastructure (PKI), etc.
- [ ] **STANDALONE PRODUCT:** the cryptographic functionality can be easily extracted for use as a standalone product
- [ ] None of the above

If you check any of the boxes above, please explain:
```
(Provide your answer here)
```

### 11. Provide any additional comments that you may have

```
(Provide your answer here)
```
