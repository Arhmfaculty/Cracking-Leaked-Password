# Cracking-Leaked-Password

## **Overview**
This project evaluates the security vulnerabilities associated with password hashing algorithms and provides actionable recommendations to enhance password protection measures. Using Hashcat, an advanced password recovery tool, a security assessment was conducted to crack passwords hashed with the MD5 algorithm. The assessment highlighted weaknesses in the current password protection system and proposed strategies to mitigate risks. 

## **Assessment Methodology**
- **Tool Used:** Hashcat, a GPU-based password recovery tool, was employed to test the strength of hashed passwords. 
- **Algorithm Tested:** MD5 hashing algorithm, which converts passwords into 32-character hashed strings, was analyzed for vulnerabilities.
- **Scope:** Focused on identifying weaknesses in hashing methods and evaluating password policies to strengthen authentication mechanisms.

## **Findings**
### **1. Vulnerability in MD5 Hashing Algorithm**
MD5 is widely recognized for its fast hashing process, which reduces computational overhead. However, this speed also makes it highly susceptible to brute-force attacks. Hackers can efficiently generate hashes using dictionary or rainbow table attacks to reverse-engineer passwords.

### **2. Password Policy Weaknesses**
The organization's current password policy permits the use of only lowercase letters and digits, without enforcing symbols or uppercase characters. It also lacks requirements for minimum length and restrictions against repeated characters, leaving passwords vulnerable to attacks.

### **3. Cracked Password Results**
![password_crack](https://github.com/user-attachments/assets/e9de0bda-4a4f-4420-bd6c-b82135e8f291)


### **4. Password Document Analysis**
![image](https://github.com/user-attachments/assets/65ddd6ef-5e10-4cfd-a37c-d004f73ad5ed)

## **Recommendations**
### **1. Upgrade to Secure Hashing Algorithms**
- Replace MD5 with slower and more secure hashing algorithms such as **bcrypt**, **scrypt**, or **Argon2**.
- These algorithms are computationally expensive, making brute-force attacks significantly more difficult.

### **2. Implement Salting Mechanism**
- Incorporate **salting** to ensure each password hash is unique, even if two users have identical passwords.
- Salting introduces additional randomness, making precomputed attacks like rainbow tables ineffective.

### **3. Strengthen Password Policies**
- Require the use of **uppercase letters**, **symbols**, and **numbers** to enforce complex passwords.
- Set a **minimum password length** of at least 12 characters.
- Prohibit **repeated characters** and common patterns.
- Enforce **regular password updates** and implement **multi-factor authentication (MFA)** for an additional layer of security.

### **4. Educate Users on Security Best Practices**
- Provide training programs on password management, phishing awareness, and recognizing social engineering tactics.
- Recommend the use of **password managers** to generate and securely store strong, unique passwords.

### **5. Continuous Monitoring and Testing**
- Conduct **regular penetration testing** to identify vulnerabilities before attackers can exploit them.
- Monitor system logs and implement **intrusion detection systems (IDS)** to detect suspicious activities.

## **Conclusion**
This project highlights the critical need to replace outdated password hashing algorithms and enforce stricter password policies to mitigate security risks. Implementing the proposed recommendations will enhance the organization's security posture and protect sensitive data from unauthorized access. Future steps include deploying a secure password manager and conducting regular security assessments to maintain resilience against evolving threats.

