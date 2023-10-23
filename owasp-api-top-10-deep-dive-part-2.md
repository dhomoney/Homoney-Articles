# **OWASP API Top 10 Deep Dive - Part Duex**

![Just Duex It!](/images/just-duex-it.jpg)

In this follow-up post to our now viral and world-famous blog, entitled with the ever catchy title [OWASP API Top 10 Deep Dive - Part 1](https://www.wwt.com/blog/owasp-api-top-10-deep-dive-part-1). Herein we will delve deeper into categories 3 and 4 on the list, Broken Object Property Level Authorization and Unrestricted Resource Consumption. Without further ado and a shiver of excitement up our spines...

## **Broken Object Property Level Authorization**

This vulnerability is the combination of two categories from the [2019 OWASP API Top Ten](https://owasp.org/API-Security/editions/2019/en/0x00-header/) as it was rightly determined this was the root cause of both vulnerabilities. The first was [Excessive Data Exposure](https://owasp.org/API-Security/editions/2019/en/0xa3-excessive-data-exposure/) which is where an API allows a user access to properties of an endpoint or object that they shouldn't have access too. 

The second previous category that is covered by Broken Object Property Level Authorization is [Mass Assignment](https://owasp.org/API-Security/editions/2019/en/0xa6-mass-assignment/) and it allows a user to modify in some way a sensitive property they should not be able to modify. 

### **What are the risks associated with Broken Object Property Level Authorization?**

Excessive data exposure in APIs can have significant consequences, as it can potentially lead to the exposure of sensitive information. This can include personally identifiable information (PII) such as names, addresses, and social security numbers, as well as more sensitive data such as financial information and health records. Furthermore, such exposure may result in identity theft, financial fraud, and other malicious activities, making it crucial to ensure that proper security measures are taken to prevent such incidents from occurring. As such, it is imperative that developers and organizations take the necessary steps to secure their APIs and protect the sensitive data that they hold, such as implementing API Security, API Sec Testing, and Secure SDLC and AppSec Orchestration & Correlation (ASOC). By doing so, they can not only safeguard their customers' sensitive information but also avoid costly data breaches and potential reputational damage.

The exploitation of mass assignment in APIs can lead to various security risks, including but not limited to privilege escalation, data tampering, and the bypassing of security mechanisms. As a result, it is important for developers to take extra precautions when designing and implementing APIs to prevent these types of attacks. Some recommended measures include implementing proper input validation and sanitization, using parameterized queries, and limiting the fields that can be updated through mass assignment. In addition, regular security audits and vulnerability assessments from API Sec Testing and SAST/DAST/IAST/SCA can help identify potential weaknesses in the API and ensure that it is secure against attacks at the code level, while API Security and Web Application and API Protection (WAAP) can provide runtime protection while development resolves issues in the code. By taking these steps, companies can help ensure the security and integrity of their APIs and protect their users' sensitive data from malicious actors.

![Secure/Defend](/images/secure-defend.jpg)

## **Unrestricted Resource Consumption**

Unrestricted Resource Consumption (URC) is a type of security vulnerability that occurs when an API does not properly limit the amount of resources that can be consumed by a single request. This can allow an attacker to overwhelm the system by sending a large number of requests that consume excessive resources. URC vulnerabilities can be particularly dangerous in APIs that provide access to sensitive or critical resources.

![Swarm Credit: FAO/Sven Torfinn](/images/swarm.jpg)

One common cause of URC vulnerabilities is the lack of rate limiting. For example, an API may allow users to make unlimited requests without any restrictions, which can lead to excessive resource consumption. This can be mitigated by implementing rate limiting, which limits the number of requests that a user can make within a certain time frame.

Another common cause of URC vulnerabilities is the lack of input validation. If an API does not properly validate user input, an attacker can send requests that contain malicious or unexpected data. This can cause the system to consume excessive resources while processing the input. Input validation can help prevent URC vulnerabilities by ensuring that only valid and expected input is processed by the API.

### **What are the risks associated with Unrestricted Resource Consumption?**

URC vulnerabilities in APIs can have serious consequences for both users and organizations. If an attacker is able to overwhelm the system with excessive requests, they can potentially cause denial of service (DoS) or distributed denial of service (DDoS) attacks. This can result in service disruptions, financial losses, and damage to reputation. In addition, URC vulnerabilities can also be used as a means of reconnaissance, allowing attackers to gather information about the system and identify other vulnerabilities.

To prevent and mitigate URC vulnerabilities, organizations should implement proper input validation and rate limiting. They should also monitor API usage for signs of excessive resource consumption and implement mechanisms to detect and block malicious requests. By taking these steps, organizations can help protect their APIs from URC vulnerabilities and ensure the security and integrity of their systems.
