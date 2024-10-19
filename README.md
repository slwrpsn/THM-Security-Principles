[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=25&pause=1000&color=2007F7&center=true&vCenter=true&width=435&lines=Security+Principles)](https://git.io/typing-svg)

![image](https://github.com/user-attachments/assets/0b2c81cc-b087-44cc-8895-ab7ddbc67901)

$\color{red}{Confidentiality}$ ensures that only the intended persons or recipients can access the data.

$\color{blue}{Integrity}$ aims to ensure that the data cannot be altered; moreover, we can detect any alteration if it occurs.

$\color{green}{Availability}$ aims to ensure that the system or service is available when needed.

### BEYOND CIA

**Authenticity:** Authentic means not fraudulent or counterfeit. Authenticity is about ensuring that the document/file/data is from the claimed source.

**Nonrepudiation:** Repudiate means refusing to recognize the validity of something. Nonrepudiation ensures that the original source cannot deny that they are the source of a particular document/file/data. This characteristic is indispensable for various domains, such as shopping, patient diagnosis, and banking.

![image](https://github.com/user-attachments/assets/b995fa51-ed63-47ec-a737-91333251da52)

$\color{red}{Disclosure}$ is the opposite of confidentiality. In other words, disclosure of confidential data would be an attack on confidentiality.

$\color{blue}{Alteration}$ is the opposite of Integrity. For example, the integrity of a cheque is indispensable.

$\color{green}{Destruction/Denial}$ is the opposite of Availability.

Consider the previous <ins>example<ins/> of patient records and related systems:

Disclosure: As in most modern countries, healthcare providers must maintain medical records’ confidentiality. As a result, if an attacker succeeds in stealing some of these medical records and dumping them online to be viewed publicly, the health care provider will incur a loss due to this data disclosure attack.

Alteration: Consider the gravity of the situation if the attacker manages to modify patient medical records. This alteration attack might lead to the wrong treatment being administered, and consequently, this alteration attack could be life-threatening.

Destruction/Denial: Consider the case where a medical facility has gone completely paperless. If an attacker manages to make the database systems unavailable, the facility will not be able to function properly. They can go back to paper temporarily; however, the patient records won’t be available. This denial attack would stall the whole facility.

We have learned that the security triad is represented by Confidentiality, Integrity, and Availability (CIA). One might ask, how can we create a system that ensures one or more security functions? The answer would be in using security models. In this task, we will introduce three foundational security models:

❇️ Bell-LaPadula Model

✳️ The Biba Integrity Model

❎ The Clark-Wilson Model

## Bell-LaPadula Model

Objective: <ins>Protect confidentiality.</ins>

Key Principles:

No Read Up (Simple Security Property): A subject at a lower security level cannot read data at a higher level.

No Write Down (*-Property): A subject at a higher security level cannot write data to a lower level, preventing leakage of sensitive information.

Use Case: Common in government and military applications where data confidentiality is paramount.

## Biba Integrity Model

Objective: <ins>Protect integrity.</ins>

Key Principles:

No Write Up: A subject at a lower integrity level cannot write to an object at a higher level.

No Read Down: A subject at a higher integrity level cannot read data from a lower level, ensuring that high-integrity subjects do not receive potentially corrupted data.

Use Case: Often applied in environments where data accuracy and reliability are critical, such as financial systems.

## Clark-Wilson Model

Objective: <ins>Ensure data integrity through well-formed transactions.</ins>

Key Principles:

Well-formed Transactions: Only authorized users can perform specific actions on data, ensuring that all modifications occur through controlled processes.

Separation of Duties: Divides responsibilities among different individuals to prevent fraud and errors.

Use Case: Frequently used in commercial systems where data integrity and consistency are essential, such as in banking systems.

[Added Information]

The Clark-Wilson Model also aims to achieve integrity by using the following concepts:

**Constrained Data Item (CDI):** This refers to the data type whose integrity we want to preserve.

**Unconstrained Data Item (UDI):** This refers to all data types beyond CDI, such as user and system input.

**Transformation Procedures (TPs):** These procedures are programmed operations, such as read and write, and should maintain the integrity of CDIs.

**Integrity Verification Procedures (IVPs):** These procedures check and ensure the validity of CDIs.

### Summary

**Bell-LaPadula** focuses on confidentiality with its read/write rules.

**Biba** prioritizes integrity, preventing corruption of data through strict access controls.

**Clark-Wilson** combines integrity with transaction controls, emphasizing controlled operations and separation of duties.
___________________________________________________________________________________________________________________________
**Defence-in-Depth** refers to creating a security system of multiple levels; hence it is also called Multi-Level Security.

## Threat VS Risk

Vulnerability: Vulnerable means susceptible to attack or damage. In information security, a vulnerability is a weakness.

Threat: A threat is a potential danger associated with this weakness or vulnerability.

Risk: The risk is concerned with the likelihood of a threat actor exploiting a vulnerability and the consequent impact on the business.

___________________________________________________________________________________________________________________________

Finally, the Shared Responsibility Model is worth mentioning, especially with the increased reliance on cloud services. Various aspects are required to ensure proper security. They include hardware, network infrastructure, operating systems, applications, etc. However, customers using cloud services have different access levels depending on the cloud services they use. For example, an Infrastructure as a Service (IaaS) user has complete control (and responsibility) over the operating system.

On the other hand, a Software as a Service (SaaS) user has no direct access to the underlying operating system. Consequently, achieving security in a cloud environment necessitates both the cloud service provider and the user to do their parts. The Shared Responsibility Model is a cloud security framework to ensure that each party is aware of its responsibility.

SEE [ISO/IEC TS 19249](https://cdn.standards.iteh.ai/samples/64140/05aa4c62ec3941a58e4156d53fad802b/ISO-IEC-TS-19249-2017.pdf) for architectural and design principles that may be used in the development of secure products, systems and applications.

