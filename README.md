# Artemis-Software
Summary: Artemis Financial's Software Requirements and Solutions

1. Who Was the Client? What Issues Did They Want Addressed?

Client: Artemis Financial, a financial institution.
Issue: Artemis Financial required a secure software application to handle sensitive data like financial transactions. The company faced vulnerabilities such as insecure communications, lack of input validation, potential SQL injection risks, and improper error handling. These issues posed risks to data confidentiality, integrity, and system reliability.
2. Identifying Security Vulnerabilities and Why Secure Coding Is Important

    What Was Done Well:
        Conducted manual code reviews and static testing to identify vulnerabilities like lack of input validation, SQL injection, and hardcoded credentials.
        Applied cryptographic hashing (SHA-256) for data integrity and secured communication using SSL/TLS encryption.

    Importance of Secure Coding:
        Data Protection: Prevents unauthorized access to sensitive client information.
        Compliance: Aligns with regulatory requirements like PCI DSS and GDPR.
        Trust: Strengthens customer confidence in the organization’s ability to protect their financial information.
        Risk Mitigation: Reduces the risk of data breaches and legal repercussions, ensuring operational continuity.

    Value to Company:
        Secure software increases customer trust, prevents costly breaches, and ensures compliance, directly contributing to the company’s overall financial well-being and reputation.

3. Challenges and Benefits of the Vulnerability Assessment

    Challenges:
        Addressing vulnerabilities in legacy code without breaking functionality.
        Managing dependencies with known vulnerabilities, like Log4j and Spring Framework.

    Helpful Aspects:
        The vulnerability assessment flow diagram guided systematic identification and prioritization of security issues.
        Tools like static dependency checks provided clear insights into known vulnerabilities and recommended fixes.

4. Increasing Layers of Security

Layers of security were added through:

    HTTPS with SSL/TLS: Encrypted communication channels.
    Input Validation: Added validation to sanitize user inputs and prevent SQL injection or XSS attacks.
    Cryptographic Hashing: Used SHA-256 for secure checksum generation.
    Error Handling: Refactored code to prevent internal information leakage.
    Secure Resource Management: Removed hardcoded credentials and implemented environment-based configuration.

Future Tools:

    OWASP ZAP and Burp Suite for penetration testing.
    SonarQube for automated static code analysis to identify vulnerabilities.
    Threat Modeling to prioritize risks and decide appropriate mitigation techniques.

5. Ensuring Functional and Secure Code

    Functionality Tests:
        Tested endpoints /hash and /checksum to ensure correct functionality of cryptographic hashing.
        Verified HTTPS connection and browser-based SSL warnings.

    Ensuring No New Vulnerabilities:
        Re-ran static analysis tools after refactoring to confirm no new vulnerabilities were introduced.
        Performed manual testing for edge cases to validate input sanitization and error handling.

6. Tools, Resources, and Practices Used

    Key Tools:
        Java Keytool: For generating SSL certificates.
        Spring Boot: For creating secure endpoints and implementing server-side security measures.
        OWASP Dependency-Check: To identify known vulnerabilities.

    Coding Practices:
        Secure coding standards like input validation, secure error handling, and encrypted communication.
        Use of prepared statements to prevent SQL injection.
        Proper keystore management and secure configurations.

7. Showcasing to Future Employers

This project demonstrates critical skills that are highly valuable in software security roles:

    Vulnerability Identification and Mitigation: Manual reviews, dependency checks, and secure code refactoring.
    Secure Coding Practices: Implementing SSL/TLS, input validation, and cryptographic hashing.
    Practical Problem-Solving: Enhancing software security without breaking functionality.
    Tools Proficiency: Experience with security tools like OWASP Dependency-Check and SSL certificate management.

By showcasing this project, I can demonstrate my ability to identify security risks, refactor code for secure operations, and implement industry-standard solutions for maintaining software integrity and security.
