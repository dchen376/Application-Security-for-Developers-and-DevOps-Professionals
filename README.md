# Application-Security-for-Developers-and-DevOps-Professionals
https://www.coursera.org/learn/application-security-for-developers-devops

## I. Introduction to Security for Application Development
- DevSecOps (Development, Security, and Operations)
- SDLC (software development Lifecycle)
  ![image](https://github.com/user-attachments/assets/f1bc7d30-0a29-4f1d-aa3a-18ee247f66ad)
- secure SDLC
  ![image](https://github.com/user-attachments/assets/3036dece-7c38-44ef-a44f-fbb1745f5c39)

- OSI model (Open Systems Interconnection Model): a conceptual framework that standardizes how network communication occurs between devices.
- seven layers of OSI
  ![image](https://github.com/user-attachments/assets/4bf6f998-19f1-40bf-a157-8b0e7c957cae)

- layers of security
  ![image](https://github.com/user-attachments/assets/422b0c6b-8644-4af0-9813-50b8ec285b14)

- security patterns
  ![image](https://github.com/user-attachments/assets/9006d5f0-089e-4b4e-a01e-ebb54b7220a5)
![image](https://github.com/user-attachments/assets/075d86bb-c100-4ade-b8eb-3224f7348380)
![image](https://github.com/user-attachments/assets/a8850394-bca5-4bae-a9b7-97282bb25cd4)

- **TLS** (Transport Layer Security)  / **SSL** (Secure Sockets Layer) -> **Modern TLS**

- vulnerability scanning
  ![image](https://github.com/user-attachments/assets/94fdd58d-f5f9-48b8-a6d4-bf358a4d0e11)
![image](https://github.com/user-attachments/assets/a7a8139a-92b8-4fc6-b939-5c7d4007d1d2)

- **threat modeling**: a proactive mitigation strategy that involves identifying, analyzing, and addressing potential security threats in an application or system during the design and development phases.
  - STRIDE (Spoofing, Tampering, Repudiation, Information Disclosure, Denial of Service, and Elevation of Privileges)
- threat monitoring: scanning code repositories and containers to find security issues.
- code checker: scans source code for security issues.

- security terminology
  ![image](https://github.com/user-attachments/assets/29a6fae9-4c38-4c34-83f4-7420ad5d0664)
- Nmap (network Mapper): open-source network scanning and security auditing tool.
![image](https://github.com/user-attachments/assets/12316163-4cc6-4503-90ca-e0891edb2b13)
![image](https://github.com/user-attachments/assets/eea8204c-c218-4194-9779-fa594f5b9ebf)
![image](https://github.com/user-attachments/assets/1549b2a5-27a3-4c12-8dea-6e1bb4231c25)
![image](https://github.com/user-attachments/assets/9192b696-884e-40f1-aa0a-9f151a53ce81)

![image](https://github.com/user-attachments/assets/9aa2d08c-0d32-412c-8449-9aaf8f78cfd0)
![image](https://github.com/user-attachments/assets/3cc2315e-7209-4ad4-9c85-0419be800373)
![image](https://github.com/user-attachments/assets/1839c18f-021a-419d-93fc-d603ccad8394)

## II. Security Testing and Mitigation Strategies

- functional **security testing**
  - Ad hoc testing: completely unstructured; involves improvised, unplanned testing without any formal test cases or documentation
  - exploratory testing: loosely structured; an unscripted, experience-based testing approach where testers actively explore the application to discover issues. 
- automated security testing types
  - unit testing
  - integration testing
  
- **static analysis**: examing all code or runtime binaries to help detect common vulnerabilities.
  - SAST (**static application security testing**): a methodical approach to analyzing source code, bytecode, or binaries for vulnerabilities without executing the application. It is a proactive technique widely used in secure software development to detect issues early in the development lifecycle.
  - **SonarQube**: for continuous code quality inspection
    ![image](https://github.com/user-attachments/assets/99b560fc-2234-4dfd-8866-17fb73af5333)
    ![image](https://github.com/user-attachments/assets/8548a5d6-c475-4f97-be1b-d32c343fb309)
  - SonarScanner

- **dynamic analysis**
  - DAST
  - OWASP's ZAP (Zed Attack Proxy): a tool wielded to uncover and guard against vulnerabilities in web applications. 
![image](https://github.com/user-attachments/assets/4f03b3b3-801f-4372-aba6-1c86f1b4ad1a)

- **code review**: Focuses on manually or automatically inspecting code for bugs or inefficiencies.
  ![image](https://github.com/user-attachments/assets/1ea65051-cd0a-46a6-8d20-b79a2e97b3db)
  *review codes at **Every Pull Request!**

- **vulnerability analysis**: focuses on identifying weaknesses or flaws in an application that could be exploited by attackers.
  - tools: SaaS platforms like **Snyk** (for securing code and dependencies)
    ![image](https://github.com/user-attachments/assets/89fafb5f-e6dd-4acc-a1be-b1929b9adbb8)
    ![image](https://github.com/user-attachments/assets/da493775-a678-450f-aea2-005f70c9c836)


  - **SCA** tools (Software Composition Analysis tools): Primarily examines open-source and third-party components for license or security issues.
  ![image](https://github.com/user-attachments/assets/ca1fdaae-17a6-45cb-a739-82714be25ea7)

  - penetration tools
  ![image](https://github.com/user-attachments/assets/3899c0f0-da37-49ef-ab41-301b4954d358)

  - defect tracking tool
  ![image](https://github.com/user-attachments/assets/94f60c34-e3cc-444e-8782-548b0aa1285b)

- vulnerability scanner -> **Jake** (by SonaType Nexus Community):  to check Python environments for vulnerabilities. While Jake is not created by or supported by Sonatype, it uses the Sonatype OSS Index.
![image](https://github.com/user-attachments/assets/4487ead0-a4ec-4048-9490-a1038afbfb20)
![image](https://github.com/user-attachments/assets/eb2044d2-4999-4945-a098-1192c7b4678b)

- **runtime protection**: a security mechanism that shields running applications against threats
  - **IAST**
  - **RASP**
  ![image](https://github.com/user-attachments/assets/f33d2ee7-d875-487b-b457-351ff61f2298)

- software component analysis (**SCA**): to better manage security and license compliance risks.
  ![image](https://github.com/user-attachments/assets/7586e3b5-ae43-489d-b37c-98dc6b5c41e3)
  ![image](https://github.com/user-attachments/assets/200ff7c9-8d75-4a17-a8fe-1862dafc050d)



 -  OWASP SCA **Dependency-checker** tool
![image](https://github.com/user-attachments/assets/c6eb861e-c90b-4895-bec4-683bec409959)

- **continuous security analysis**: the ongoing integration and testing of security in the SDLC.



## III. OWASP (Open Web Application Security Project) Application Security Risks

![image](https://github.com/user-attachments/assets/f844b9a3-934b-43dc-898c-aa6eb13011c6)

- sql injections
- cross site scripting
  ![image](https://github.com/user-attachments/assets/2cfbded1-7e51-455b-baf6-10408fc287a8)
- secrets management
  ![image](https://github.com/user-attachments/assets/a8e49d1d-034b-4a52-a5bb-d7361d99d34d)
    - vault (token-based secret management solution)
    - Hashicorp Vault


## IV. Security Best Practicies
- Code practices
  ![image](https://github.com/user-attachments/assets/5733fa90-6454-4701-9b6e-5c802c1be017)
  -  HTTP security headers with **flask-talisman**
  -  cross-origin resource sharing (CORS) policies using **flask-Cors**
  -  software dependencies
  -  vulnerability scan 
- Dependencies
![image](https://github.com/user-attachments/assets/09cc7467-e942-47fd-82b2-c8ef63ff3b6b)




