# API Security and ASPM - A More Perfect Union

![A More Perfect Union](/images/apisec-aspm-wedding.jpg)

In today's highly interconnected and rapidly evolving digital landscape, Application Programming Interfaces (APIs) have become an essential and indispensable component of modern software systems. APIs act as a bridge, facilitating seamless communication, data exchange, and integration between various software applications and systems. APIs enable organizations to unlock the full potential of their software resources and create innovative solutions by allowing different applications to interact and share information.

Digital Transformation continues to be a focus for most organizations while innovation becomes the differentiator. Applications and APIs are what drives the modern economy, from the products we use (mobile devices), the services we consume (banking, airline, eCommerce), and even the cars we drive. However, as the reliance on APIs continues to grow, so does the attack surface and the risk of cyber threats targeting these interfaces. Organizations must recognize the critical importance of API security and take proactive measures to safeguard sensitive data and protect the integrity of their systems. By implementing robust API security measures, organizations can mitigate the risk of unauthorized access, business logic abuse, data breaches, and malicious attacks that can have devastating consequences. Additionally, API Security alone isn't good enough

As we've discussed before in previous articles on API security, we have focused on the main security threats to APIs, as elucidated by the [OWASP Foundations'](https://owasp.org) API Top Ten for 2023 [OWASP API Top Ten 2023](https://www.wwt.com/blog/owasp-api-top-ten-2023-all-your-api-vulnerabilities-are-belong-to-us). In the market today, API Security means two essential things:

1. **API Discovery and Detection**: Find the APIs you don't know about, such as shadow and zombie APIs. You can't secure that which you don't know exists. 
2. **API Posture Management**: Understanding the vulnerabilities that exist in your APIs and the severity thereof. 

Most API Security platforms do other functions like report generation, logging, and alerting, and some even dip their toes into remediation, but the above two things are the core of what API Security is and also are the first things implemented. Is this enough though? While APIs can be the entire application, they are often a part of the application. Understanding the entire security posture of an application is better than just a part of it. This is where Application Security Posture Management (ASPM) comes into play. 

# What is Application Security Posture Management? 

In today's rapidly evolving digital landscape, organizations face a myriad of complex challenges when it comes to ensuring the utmost security of their applications and APIs. With the ever-growing number and sophistication of cyber threats lurking in the shadows, coupled with the potentially catastrophic impact of data breaches, organizations are compelled to place application security at the forefront of their priorities. Organizations must adopt a comprehensive and holistic approach to managing application and API security, and one highly effective approach is through the implementation of Application Security Posture Management (ASPM).

ASPM encompasses a wide range of activities that revolve around the continuous monitoring, assessment, and improvement of an organization's application security posture. This entails the deployment of cutting-edge strategies, streamlined processes, and state-of-the-art tools to proactively identify vulnerabilities, meticulously assess risks, and expedite the prioritization of remediation efforts, which is key in today's landscape. In most cases, ASPM solutions help prioritize vulnerabilities based on business logic, governance, risk, and compliance. Helping organizations remediate vulnerabilities faster, but more importantly, it allows them to focus on the vulnerabilities that pose an actual risk to the organization. 

## How Application Security Posture Management (ASPM) and API Security Work Together

The 2020's ever-evolving digital landscape, companies are confronted with a plethora of challenges when it comes to safeguarding the security of their data [being accessed through] contained within applications and APIs. It is crucial to address these challenges to strengthen the organization's overall security posture and safeguard valuable and confidential data.

One crucial aspect in this regard is Application Security Posture Management (ASPM), which entails the continuous monitoring, assessment, and enhancement of an organization's application security posture. By actively focusing on ASPM, organizations can proactively identify vulnerabilities and improve their overall security measures from code to runtime, regardless of where the workloads are running.

Additionally, API security plays a vital role in ensuring a robust security framework. Specifically, API security is dedicated to the protection of Application Programming Interfaces (APIs), which serve as the bridge for communication and integration between different software systems both internally and with external customers and business partners. By implementing robust security measures for APIs, organizations can effectively mitigate the ever-increasing risks associated with unauthorized access, data breaches, and malicious activities.

Together, both ASPM and API security can help establish a comprehensive security strategy that addresses the unique challenges posed by the digital landscape and guarantees the confidentiality, integrity, and availability of their applications and sensitive data.

# Two Leaders Come Together

It is exciting to hear of the technical alliance between leaders like [Akamai](https://akamai.com) and [Apiiro](https://apiiro.com) bringing these two technologies together. It was exciting news when we heard that Akamai had purchased Neosec to enhance their API security offering [Akamai API Security](https://www.akamai.com/products/api-security), augmenting their industry-leading Web Application and API Security (WAAP) product, but with this technical alliance between Akamai and Apiiro, this takes it to a whole new level. Additionally, Apiiro with their ASPM platform can now ingest runtime findings from Akamai API Security and combine this with their code-based API security capabilities allowing for the rich context needed to:

- Reduce the mean time to remediation (MTTR) of critical API risks.
- Prevent API weaknesses from being deployed to production, saving valuable time proactively vs. reactively addressing risk.
- Modernize your application risk assessment processes that are based on self-attestation questionnaires by proactively triggering reviews based on risky material API changes in code.
- Prioritize business-critical API security issues, reduce false positives, and save time triaging backlogs and fixing risks. 
- Minimize API security testing gaps and ensure more complete coverage.
- Quickly identify the app and API owners, dependencies, and audit trails for compliance. 

## A Highlight

A further and more in-depth article will be forthcoming, but let us whet your appetite though. Let's take a look at how Apiiro's ASPM Platform can correlate code and runtime findings from Akamai API Security. 

Runtime API security solutions like Akamai API Security give security teams real-time detection of vulnerable APIs and business logic abuse. But when an API vulnerability is detected, tying it back to the code and the person or team responsible for fixing it can be easier said than done. 

This integration makes that process smoother so that when API risks are detected in Akamai, security teams now have full visibility into code context from Apiiro—including the root cause, the repository it’s located in, the specific line of code, and the associated code owner.

![Event Correlation](/images/apiiro-akamai-corolation.gif)

Layering runtime and code context gives application security and development teams an accurate understanding of what is a real risk and ultimately helps reduce the mean time to remediation (MTTR) of critical API risks to your business.

