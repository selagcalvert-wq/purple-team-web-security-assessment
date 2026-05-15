# purple-team-web-security-assessment
## **Objective**

The Purple Team Web Application Security Assessment project aimed to demonstrate and analyze common web application vulnerabilities in a controlled lab environment. The primary focus was to perform coordinated offensive and defensive testing against an intentionally vulnerable web application, with red team activities used to identify and exploit weaknesses and blue team analysis used to understand detection opportunities, attack visibility, and remediation strategies.

This project provided hands-on experience with web application security testing, HTTP request manipulation, vulnerability assessment, and purple team collaboration. As Team Lead and Red Team Lead, I directed team efforts, provided walkthroughs and troubleshooting support, and personally executed 12 attacks across SQL injection, cross-site scripting, and broken authentication categories.

As part of the blue team, my responsibilities focused on analyzing attack activity, reviewing application behavior, and supporting detection and remediation efforts throughout the assessment. I assisted with monitoring how vulnerabilities and malicious requests appeared within the application and network traffic, while also helping document findings and defensive recommendations.

My role included:
-Reviewing HTTP requests and responses to better understand attack behavior and application weaknesses
-Using Browser DevTools and Wireshark to analyze network traffic, requests, responses, tokens, and client-side behavior
-Assisting with identifying indicators of SQL injection, cross-site scripting (XSS), and broken authentication activity
-Supporting documentation of vulnerabilities, findings, impact, and remediation recommendations
-Collaborating with team members during troubleshooting, testing validation, and analysis activities
-Contributing to the overall purple team workflow by helping connect offensive testing with defensive analysis and visibility

## **Skills Learned**

- Practical understanding of web application security testing concepts.
- Hands-on experience identifying and demonstrating SQL injection vulnerabilities.
- Hands-on experience identifying and demonstrating cross-site scripting vulnerabilities.
- Improved understanding of broken authentication and account lifecycle weaknesses.
- Proficiency in using Burp Suite to intercept, inspect, modify, and replay HTTP requests.
- Experience using Browser DevTools to analyze application behavior, requests, tokens, and client-side functionality.
- Practical exposure to Wireshark for reviewing network traffic and understanding attack visibility.
- Ability to document attack paths, findings, impact, and remediation recommendations.
- Improved understanding of how offensive activity can support blue team detection and alerting.
- Development of technical leadership, mentoring, troubleshooting, and team coordination skills.

## **Tools Used**

- Burp Suite for intercepting, modifying, and replaying HTTP requests.
- Browser DevTools for inspecting client-side behavior, API requests, tokens, and application responses.
- Wireshark for network traffic analysis and packet review.
- OWASP Juice Shop / intentionally vulnerable web application lab environment for controlled testing.
- Web browser for interacting with the application and validating attack behavior.
- Documentation tools for organizing findings, screenshots, explanations, and remediation recommendations.

## **Steps**

### **Project Environment Setup:**

First we hosted OWASP Juice Shop on one of our virtual machines and connected multiple other virtual machines to it using TailScale.

### **SQL Injection Testing:**

These screenshots shows SQL injection testing being performed against a vulnerable input field or API endpoint. The objective was to demonstrate how unsanitized user input could alter backend database queries in the controlled lab environment.

<img width="494" height="388" alt="Screenshot 2026-04-15 123310" src="https://github.com/user-attachments/assets/b610a272-ebda-421b-a874-3641cf1852ea" />
<img width="266" height="196" alt="Screenshot 2026-04-15 123346" src="https://github.com/user-attachments/assets/c95c3bf7-78ee-4e84-8a4a-ee00311bc786" />
<img width="409" height="297" alt="Screenshot 2026-04-15 123750" src="https://github.com/user-attachments/assets/12fdb9b6-1d83-4ae7-9d03-d12ae360cdb9" />
<img width="549" height="528" alt="Screenshot 2026-04-15 124259" src="https://github.com/user-attachments/assets/ede83539-7b5a-4bef-a0bf-a374c15ba9ac" />
<img width="1901" height="730" alt="Screenshot 2026-04-15 124358" src="https://github.com/user-attachments/assets/741ce536-1e80-4d9e-9075-79ca650d2b87" />
<img width="429" height="644" alt="Screenshot 2026-04-15 124647" src="https://github.com/user-attachments/assets/f05ef11a-d3ec-4c83-bb0d-20d36e10deeb" />

### **SQL Injection Result:**

The results demonstrated how vulnerable query logic could expose or manipulate application data when proper input validation and parameterized queries are not used.

### **Cross-Site Scripting Payload Testing:**

These screenshots shows cross-site scripting testing against a vulnerable field or endpoint. The purpose was to demonstrate how unsafe handling of user-controlled input could allow script execution in the browser.

<img width="1863" height="613" alt="Screenshot 2026-04-15 115427" src="https://github.com/user-attachments/assets/dc4689b0-1879-4f5f-996c-4cdddbe12211" />
<img width="1627" height="598" alt="Screenshot 2026-04-15 115604" src="https://github.com/user-attachments/assets/a528808f-9a4c-4185-aebe-bc1684611def" />
<img width="748" height="620" alt="Screenshot 2026-04-15 120021" src="https://github.com/user-attachments/assets/3bf3e881-2ecd-4c8f-a712-a3c495ccdd6b" />
<img width="1408" height="566" alt="Screenshot 2026-04-15 120853" src="https://github.com/user-attachments/assets/b1d825d9-a1a3-4fa5-9114-bf24babf70b9" />
<img width="1417" height="623" alt="Screenshot 2026-04-15 121106" src="https://github.com/user-attachments/assets/c167eabc-5dda-42be-b5bf-c9faf389f492" />
<img width="1833" height="707" alt="XSStest1soundcloudPayLoad" src="https://github.com/user-attachments/assets/c0849d1d-8d34-47d2-967a-60ee119a119d" />
<img width="1032" height="262" alt="frame number" src="https://github.com/user-attachments/assets/84293b23-5f75-4492-913b-d3aec7585b69" />

### **Cross-Site Scripting Execution:**

The finding demonstrated the importance of output encoding, input validation, and secure rendering of user-controlled data.

### **Broken Authentication Testing:**

These screenshots shows testing against an authentication or account management workflow. The objective was to identify weaknesses in authentication logic, session handling, account lifecycle controls, or password management behavior.

<img width="578" height="577" alt="Screenshot 2026-04-15 093335" src="https://github.com/user-attachments/assets/dbf3dc92-2b8e-48ad-b6e0-143176163e58" />
<img width="1038" height="93" alt="Screenshot 2026-04-15 093445" src="https://github.com/user-attachments/assets/920c87c2-3d74-427c-ba9f-3f60c6df55ae" />
<img width="420" height="297" alt="Screenshot 2026-04-15 093506" src="https://github.com/user-attachments/assets/a2f3bc8f-2f4a-418b-be5c-4ecc4c3f7198" />
<img width="1056" height="198" alt="Screenshot 2026-04-15 094129" src="https://github.com/user-attachments/assets/21a2370f-f663-46de-b79a-303e8d3ac898" />
<img width="407" height="452" alt="Screenshot 2026-04-15 094344" src="https://github.com/user-attachments/assets/215f749e-663d-418d-9810-238dc2bdd4fe" />
<img width="1422" height="772" alt="Screenshot 2026-04-15 094451" src="https://github.com/user-attachments/assets/8745f646-8bf4-42d3-8740-2aa29e1b0114" />
<img width="1889" height="283" alt="Screenshot 2026-04-15 101950" src="https://github.com/user-attachments/assets/3464c7d9-0f65-4839-a79b-492c3c9f3afa" />
<img width="1877" height="224" alt="Screenshot 2026-04-15 103559" src="https://github.com/user-attachments/assets/25099b72-2700-45ec-991f-3dc89f77ce42" />
<img width="991" height="596" alt="Screenshot 2026-04-15 110125" src="https://github.com/user-attachments/assets/24983671-d4e3-49fa-bef0-b84759fb4594" />
<img width="621" height="425" alt="Screenshot 2026-04-15 110218" src="https://github.com/user-attachments/assets/ba76f574-4522-4dbf-8f5d-c9e03190a994" />
<img width="1806" height="835" alt="Screenshot 2026-04-15 110311" src="https://github.com/user-attachments/assets/bb26acb5-a03a-4b3e-be7f-83ec15fda51f" />

### **Broken Authentication Result:**

The findings demonstrated how weak authentication logic could potentially allow unauthorized access, improper account changes, or abuse of account management functionality.

### **Browser DevTools Analysis**

These screenshots show Browser DevTools being used to inspect requests, responses, application storage, or client-side behavior. DevTools helped support testing by revealing how the application handled data in the browser. We were also able to use a team member's prior software dev knowledge of backend environments to craft a specific GET request to change passwords.

<img width="1056" height="198" alt="Screenshot 2026-04-15 094129" src="https://github.com/user-attachments/assets/e241ad69-f049-4b49-b0ba-3b9b0afce9d0" />
<img width="1889" height="283" alt="Screenshot 2026-04-15 101950" src="https://github.com/user-attachments/assets/d20115c7-d70f-4930-9f12-73d156000db7" />
<img width="1877" height="224" alt="Screenshot 2026-04-15 103559" src="https://github.com/user-attachments/assets/0c135ce9-82ec-4f94-86b3-9df744db0044" />

### **Final Project Documentation**

https://drive.google.com/file/d/1DI645P2yMJY6_3jHmfKJgzom-5_fQF1D/view?usp=sharing
