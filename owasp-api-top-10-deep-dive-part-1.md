# OWASP API Top 10 Deep Dive - Part 1

In this blog post, we will be taking a closer look at the [OWASP Top 10 API Security Risks](https://owasp.org/API-Security/editions/2023/en/0x11-t10/) a comprehensive list of the most critical API security risks facing organizations today. As organizations increasingly rely on APIs to power their applications, securing these APIs has become more important than ever.

If you're new here, please refer to [my previous post](https://www.wwt.com/blog/owasp-api-top-ten-2023-all-your-api-vulnerabilities-are-belong-to-us) for an introduction. In this series of deeper dive blog posts, we will be examining each of these risks in detail, starting with the first category.

By providing a deeper dive into each risk category, we hope to raise awareness of the importance of API security and provide actionable insights that organizations can use to secure their APIs. So, whether you're responsible for securing APIs within your organization or are simply interested in learning more about API security, this series of blog posts is for you.

Without further ado, let's dive into the first category of the OWASP Top 10 API Security Risks.

## **Broken Object Level Authorization**

APIs, on average, expose more endpoints or objects than traditional web applications. Today, both mobile and web-based applications are often mere skins/front-ends to APIs, providing a pleasant viewing experience for human eyes. Object Level Authorization is the code in the application that determines whether a user should have access to object in question. 

One of the challenges with object level authorization is that it can be difficult to properly manage and enforce, particularly as APIs become more complex and expose a larger number of objects. This can make it more difficult for developers to properly implement and test object level authorization, which can leave APIs vulnerable to attack.

### **What are the risks associated with Broken Object Level Authorization?**

When object level authorization is broken, attackers can gain access to sensitive information or unintended access to API functionality. This can lead to data breaches, system compromises, and other security incidents. Object level authorization is a key component of securing systems and protecting valuable data.

![Hacker](/images/hacker.jpg)

One real life example is a car manufacturer (whose name we will not mention) with an API that allowed users to remote start and stop their vehicles, lock and unlock the doors, and several other functions. As part of this, the API request was sent with the Vehicle Identification Number, or VIN, but did not ensure that the user was the owner of said VIN, allowing anyone with the VIN for the car to control the car without proper authorization, only the VIN. 

## **Broken Authentication**

The second risk category in the OWASP Top 10 API Security Risks is Broken Authentication, which can occur when authentication mechanisms are not implemented or configured properly. As APIs become more interconnected and complex, the risks associated with Broken Authentication continue to increase. Even password reset/forgotten password objects need to be treated as authentication objects. 

OWASP defines an API as vulnerable to Broken Authentication if it contains one of the following issues.  [1](https://owasp.org/API-Security/editions/2023/en/0xa2-broken-authentication/)

1. Permits credential stuffing where the attacker uses brute force with a list of valid usernames and passwords.
2. Permits attackers to perform a brute force attack on the same user account, without presenting captcha/account lockout mechanism.
3. Permits weak passwords.
4. Sends sensitive authentication details, such as auth tokens and passwords in the URL.
5. Allows users to change their email address, current password, or do any other sensitive operations without asking for password confirmation.
6. Doesn’t validate the authenticity of tokens.
7. Accepts unsigned/weakly signed JWT tokens.
8. Doesn’t validate the JWT expiration date.
9. Uses plaintext or weakly hashed passwords.
10. Uses weak encryption keys.

Additionally, OWASP states that microservices -- which are often associated with APIs -- are vulnerable if the following conditions exist:

1. Other microservices can access it without authentication.
2. Uses weak or predictable tokens to enforce authentication.

![Anonymous](/images/anonymous-hacker.jpg)

### **What are the risks associated with Broken Authentication?**

The risks associated with Broken Authentication are similar to those of Broken Object Level Authorization: attackers can gain access to sensitive information or functionality to which they are not authorized. However, Broken Authentication refers specifically to issues with the authentication mechanisms used to verify identity.

For example, if an API does not properly authenticate clients (either human users or machine-to-machine access,) an attacker can use stolen token to gain unauthorized access to the system. Additionally, if the authentication mechanism is weak or easily bypassed, an attacker could exploit this vulnerability to gain access. While this typically requires more skill on the part of the attacker, the payoff is usually greater.
