# OWASP API Top Ten Deep Dive Part 3

In this blog post, we continue the deep dive into the 2023 release of the [OWASP API Top Ten](https://www.wwt.com/blog/owasp-api-top-ten-2023-all-your-api-vulnerabilities-are-belong-to-us) with part 3 covering Broken Function Level Authorization and Unrestricted Access to Sensitive Business Flows, numbers 5 and 6 respectively on the list. While Broken Function Level Authorization isn't new, Unrestricted Access to Sensitive Business Flows is unique to the 2023 list and shows the ever-changing landscape and attack vectors used with the growing adoption of APIs today. 

Unrestricted Access to Sensitive Business Flows is where all the differentiation and development is going in runtime API security products today. While WAF/WAAP can do protections based upon HTTP/HTML effectively, they need more insight and a deep understanding of the APIs required to fully secure APIs and the data behind them. 

## Broken Function Level Authorization in APIs

When it comes to securing APIs, one of the critical aspects to consider is function-level authorization. Function level authorization determines which users or roles can access specific API endpoints or functions. However, if this authorization mechanism is not implemented correctly, it can lead to a severe security vulnerability known as Broken Function Level Authorization. This blog post will explore what Broken Function Level Authorization is and why it is a problem.

Broken Function Level Authorization occurs when an API does not correctly enforce authorization checks for different functions or endpoints. This means that even if a user is not authorized to perform a specific action, they may still be able to access and execute it through the API. Essentially, this vulnerability allows unauthorized users to bypass security controls and perform activities they shouldn't be able to.

![coding](/images/coding.jpg)

### Risks associated with Broken Function Level Authorization?

Broken function-level authorization can have severe consequences for an API's and its users' security. By exploiting this vulnerability, attackers can gain unauthorized access to sensitive data or perform actions that should only be allowed for privileged users. For example, a user with limited access might be able to escalate their privileges and gain administrative rights, compromising the entire system. Additionally, it can lead to data breaches, unauthorized modifications, or even complete system compromise.

Function-level authorization is a critical component of API security. Failure to implement proper authorization checks can result in Broken Function Level Authorization, allowing unauthorized users to exploit the API. To prevent this vulnerability, it is essential to implement robust authorization mechanisms such as RBAC or ABAC and regularly audit the API's security. By doing so, you can ensure your API's confidentiality, integrity, and availability and the data it handles.

## Unrestricted Access to Sensitive Business Flows

In the realm of API security, one of the critical concerns is ensuring restricted access to sensitive business flows. The concept of restricted access revolves around determining which users or roles are authorized to perform specific actions within an API. However, if this access control mechanism needs to be correctly implemented, it can lead to a significant security vulnerability known as Unrestricted Access to Sensitive Business Flows. This blog post will delve into what Unrestricted Access to Sensitive Business Flows entails, why it poses a threat, and how to mitigate this risk.

Unrestricted Access to Sensitive Business Flows occurs when an API needs to enforce proper access controls for critical business flows or processes. Even unauthorized users can execute sensitive actions or access confidential information through the API. This vulnerability enables malicious actors to bypass security measures and perform actions only accessible to authorized individuals.

![You've Been Hacked](/images/youve-been-hacked.jpg)

### Risks Associated with Unrestricted Access to Sensitive Business Flows

Unrestricted Access to Sensitive Business Flows can have dire consequences for the API and its users. Exploiting this vulnerability can enable attackers to gain unauthorized entry to sensitive data or perform actions that should be restricted to privileged users. For instance, an unauthorized user might gain access to financial transactions, customer data, or proprietary information, leading to economic loss, reputational damage, or legal implications. Additionally, it can result in business disruption, regulatory compliance violations, or even compromise the entire system.

Proper implementation of access controls is crucial to API security. Neglecting to enforce adequate restrictions can result in Unrestricted Access to Sensitive Business Flows, granting unauthorized users the ability to exploit the API's functionalities. To mitigate this vulnerability, it is paramount to implement robust access control mechanisms such as Role-Based Access Control (RBAC) or Attribute-Based Access Control (ABAC). Additionally, performing regular security audits and assessments of the API can help identify and rectify potential vulnerabilities. By adopting these measures, organizations can safeguard the confidentiality, integrity, and availability of their APIs and the sensitive data they handle.
