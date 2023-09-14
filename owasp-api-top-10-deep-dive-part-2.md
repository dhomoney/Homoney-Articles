# **OWASP API Top 10 Deep Dive - Part Duex**

![Just Duex It!](/images/just-duex-it.jpg)

In this follow up post to our now viral and world famous blog, entitled with the ever catchy title "OWASP API Top 10 Deep Dive - Part 1". Herein we will delve deeper into categories 3 and 4 on the list, Broken Object Property Level Authorization and Unrestricted Resource Consumption. Without futher ado and a shiver of excitement up our spines...

## **Broken Object Property Level Authorization**

Broken Object Level Authorization (BOLA) is a type of security vulnerability that occurs when an application does not properly enforce access controls for object properties. This can allow an attacker to access or modify sensitive information that they should not have access to. BOLA vulnerabilities can be particularly dangerous in APIs, where the attacker can potentially access data from multiple users.

One common cause of BOLA vulnerabilities in APIs is the use of overly-permissive access controls. For example, an API may allow a user to view their own account information, but fail to properly restrict access to other users' account information. This can allow an attacker to access sensitive data by simply changing the ID of the account they are trying to access.

Another common cause of BOLA vulnerabilities is the use of insecure object references. In some cases, an application may use an object's ID as a reference to that object throughout the application. If an attacker can guess or manipulate the ID of an object, they can potentially access or modify the properties of that object.

### **What are the risks associated with Broken Object Property Level Authorization?**

BOLA vulnerabilities in APIs can have serious consequences for both users and organizations. If an attacker is able to access or modify sensitive information through a BOLA vulnerability, they can potentially steal user data or compromise the integrity of the application. This can result in financial losses, damage to reputation, and legal liabilities.

In addition to direct harm to users and organizations, BOLA vulnerabilities can also have indirect consequences. For example, if an attacker is able to steal user data, they can potentially use that data in targeted phishing attacks or identity theft. This can further harm users and damage the reputation of the organization. Therefore, it is important for organizations to take BOLA vulnerabilities seriously and take steps to prevent and mitigate them.

## **Unrestricted Resource Consumption**

Unrestricted Resource Consumption (URC) is a type of security vulnerability that occurs when an API does not properly limit the amount of resources that can be consumed by a single request. This can allow an attacker to overwhelm the system by sending a large number of requests that consume excessive resources. URC vulnerabilities can be particularly dangerous in APIs that provide access to sensitive or critical resources.

![Swarm Credit: FAO/Sven Torfinn](/images/swarm.jpg)

One common cause of URC vulnerabilities is the lack of rate limiting. For example, an API may allow users to make unlimited requests without any restrictions, which can lead to excessive resource consumption. This can be mitigated by implementing rate limiting, which limits the number of requests that a user can make within a certain time frame.

Another common cause of URC vulnerabilities is the lack of input validation. If an API does not properly validate user input, an attacker can send requests that contain malicious or unexpected data. This can cause the system to consume excessive resources while processing the input. Input validation can help prevent URC vulnerabilities by ensuring that only valid and expected input is processed by the API.

### **What are the risks associated with Unrestricted Resource Consumption?**

URC vulnerabilities in APIs can have serious consequences for both users and organizations. If an attacker is able to overwhelm the system with excessive requests, they can potentially cause denial of service (DoS) or distributed denial of service (DDoS) attacks. This can result in service disruptions, financial losses, and damage to reputation. In addition, URC vulnerabilities can also be used as a means of reconnaissance, allowing attackers to gather information about the system and identify other vulnerabilities.

To prevent and mitigate URC vulnerabilities, organizations should implement proper input validation and rate limiting. They should also monitor API usage for signs of excessive resource consumption and implement mechanisms to detect and block malicious requests. By taking these steps, organizations can help protect their APIs from URC vulnerabilities and ensure the security and integrity of their systems.