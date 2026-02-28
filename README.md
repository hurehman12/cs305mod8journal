Artemis Financial Vulnerability Assessment

Artemis Financial is a financial consulting company that develops individualized financial plans for its clients, including savings, retirement, investment, and insurance strategies. The company uses a web-based RESTful application to manage sensitive financial and personal data. 
My task was to conduct a vulnerability assessment to identify security weaknesses and recommend mitigation strategies to protect client information.

Security Vulnerabilities Identified:

1- Through manual code review, I identified issues such as:

2- Hardcoded database credentials

3- Use of root database privileges

4- Missing authentication and authorization controls

5- Lack of input validation

6- Insecure exception handling

Using OWASP Dependency-Check, I identified 148 known vulnerabilities across third-party dependencies, including critical vulnerabilities in Spring Framework, Tomcat, Jackson, SnakeYAML, and other libraries. Several were marked as known exploited vulnerabilities.

One of the most challenging parts of this assessment was analyzing the large number of CVEs and determining which vulnerabilities posed the highest risk. It was helpful to see how upgrading a core framework like Spring Boot could resolve many transitive dependency issues at once.

This project reinforced the importance of coding securely, especially when handling financial data. Secure coding protects confidentiality, integrity, and availability while reducing legal, financial, and reputational risk for a company.

Security Improvements and Mitigation:

To mitigate risks, I recommended:

1- Upgrading outdated dependencies

2- Removing hardcoded credentials

3- Implementing least-privilege database access

4- Enforcing HTTPS/TLS communication

5- Implementing authentication and role-based authorization

6- Validating and sanitizing user input

7- Integrating dependency scanning into CI/CD pipelines

After refactoring and applying mitigation strategies, I re-ran dependency scans and reviewed the application to ensure functionality remained intact and no new vulnerabilities were introduced.

These improvements significantly strengthen the overall security posture of the system.

Tools and Practices Used:

1- OWASP Dependency-Check (Maven plugin)

2- CVE and NVD vulnerability analysis

3- Spring Boot dependency management

4- Secure coding best practices

5- Manual code review techniques


In the future, I would also use additional tools such as OWASP ZAP for dynamic testing and automated static analysis tools to further strengthen application security.


Value to Employers

This project demonstrates my ability to:

1- Perform structured vulnerability assessments

2- Analyze and interpret CVE data

3- Identify insecure coding practices

4- Develop practical mitigation strategies

5- Apply layered security principles in modern web applications

This artifact shows hands-on experience in secure software development and risk mitigation within a real-world application scenario.






