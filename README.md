# cs305mod8journal
This repo contains cs305 mod 8 reflection


Artemis Financial is a financial consulting company that develops individualized financial plans for its clients, including savings, retirement, investment, and insurance strategies. The company uses a web-based RESTful application to manage sensitive financial and personal data. My task was to conduct a vulnerability assessment to identify security weaknesses and recommend mitigation strategies to protect client information.

Security Vulnerabilities Idewntified
Through manual code review, I identified issues such as:
-Hardcoded database credentials
-Use of root database privileges
-Missing authentication and authorization controls
-Lack of input validation
-Insecure exception handling

Using OWASP Dependency-Check, I identified 148 known vulnerabilities across third-party dependencies, including critical vulnerabilities in Spring Framework, Tomcat, Jackson, SnakeYAML, and other libraries. Several were marked as known exploited vulnerabilities. This assessment highlighted the importance of maintaining secure coding practices and regularly updating dependencies.

Security Improvements and Mitigation
To mitigate risks, I recommended:
-Upgrading outdated dependencies
-Removing hardcoded credentials
-Implementing least-privilege database access
-Enforcing HTTPS/TLS communication
-Implementing authentication and role-based authorization
-Validating and sanitizing user input
-Integrating dependency scanning into CI/CD
These steps significantly improve confidentiality, integrity, and availability of the system.

Tools and Practices Used
-OWASP Dependency-Check (Maven plugin)
-CVE and NVD vulnerability analysis
-Spring Boot dependency management
-Secure coding best practices
-Manual code review techniques

Value to Employers
This project demonstrates my ability to:
-Perform structured vulnerability assessments
-Analyze and interpret CVE data
-Identify insecure coding practices
-Develop mitigation strategies
-Apply layered security principles in modern web applications
It reflects practical experience in secure software development and risk mitigation.
