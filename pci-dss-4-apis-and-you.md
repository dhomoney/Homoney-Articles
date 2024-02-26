# PCI DSS 4, APIs, and You - The Ostrich is Looking Around

![PCI on API Security before 4.0](/images/ostrich-head-in-ground.jpg)

If you hadn't heard the news, the Payment Card Industry (PCI) Security Standards Committee (SSC) Data Security Standards (DSS) have been updated and come into effect on March 31st, 2024. This is a major update that corrects some of the sins of the past and drives home the need to "shift left" with security and also regulates APIs by name. This is a huge difference from the previous PCI DSS standard of 3.2.1, over 50 between the two. Until now PCI DSS was the proverbial Ostrich with it's head buryed. In this post we are going to discuss broadly the changes, specifically in section 6 of PCI DSS 4, and how the PCI SSC has pulled it's head out of the sand in a big way.

## Requirement 6

Requirement 6 of the upcoming new PCI DSS 4.0 stardard states the following:

> Code repositories that store application code, system configurations, or other configuration data that can
> impact the security of account data or the CDE are in scope for PCI DSS assessments.

This marks the first time that all code repositories are now in-scope for PCI DSS audit and security requirements. Additionally, we would be remiss if we didn't call something out. Throughout Requirement 6 of PCI DSS 4.0 you will oft see repeated the phrase "Bespoke and custom software". The passage pertains to custom code, which can either be internally developed by your organization or supplied by an external party. This code is governed by the requirements set forth in the Data Security Standard (DSS). Specifically, we need to consider the following scenarios:

1. **Account Data Handling**: If the custom software interacts with account data, whether by storing, processing, or transmitting it, it falls squarely within the purview of these DSS requirements. The security of account data is paramount, and any software that touches it must adhere to the stipulated guidelines.
2. **APIs Included**: Notably, this definition extends to Application Programming Interfaces (APIs). Therefore, if your bespoke and tailor-made software integrates APIs—whether for data exchange, communication, or functionality—these APIs are also subject to the same scrutiny.
3. **Holistic Review**: As we delve into the specifics of DSS version 4.0, it’s essential to recognize that the requirements apply not only to the custom-developed applications themselves but also to any APIs they incorporate. In other words, if a particular requirement is relevant to your software, it equally pertains to the APIs woven into its fabric.

What PCI is trying to foster and encourage is a culture of security across the board. No longer is SecOps the sole party responsible for securing all the things. This involves making security fundimental to developments requiring them to implement code testing and review, secure code practices, and remediation before code is released to production. 

With the basics out of the way, let's delve down into PCI DSS 4.0 to see what else pertains to API Security. 

## With Titles Like This, Who Need Ambien?

![PCI DSS 4: Kitty Ambien](/images/sleeping-kitten.jpg)

We will now delve into Section 6.2 of PCI DSS 4.0, which has the riveting title "Bespoke and custom software are developed securely", a real page turner of a title, but this section has some real heavy hitting requirements one must be aware of. Let's start with the first sub-section 6.2.1.

### Section 6.2.1

1. **Requirement 6.2.1**:
   - The text refers to a specific requirement, namely **6.2.1**. In the context of the **Payment Card Industry Data Security Standard (DSS)**, this requirement holds significance. It serves as a guiding principle for organizations aiming to safeguard sensitive data.
   - The essence of this requirement lies in the need to **comprehend how sensitive data is handled within an application**. This understanding forms the bedrock upon which protective measures can be effectively implemented.

2. **APIs and Their Implications**:
   - The passage explicitly highlights the relevance of **Application Programming Interfaces (APIs)**. These APIs act as conduits for data exchange, communication, and functionality within software systems.
   - The **clear implication** here is that the **Payment Card Industry (PCI)** emphasizes the integration of **security measures from the outset**. In other words, organizations should **"shift left"**—a term often used to describe early-stage security integration.
   - The concept of **"baking in" security** underscores the need to address security concerns **during the initial development phases** rather than attempting to retrofit security later. This proactive approach ensures that security considerations are **inherent to the software's design**.

3. **APIs and Custom Code**:
   - When crafting **custom code**, whether it's internally developed or received from external sources, organizations must **adhere to DSS requirements**. These requirements extend beyond the application itself to encompass any APIs woven into its fabric.
   - The **by-design approach** is pivotal. Rather than treating security as an afterthought, organizations should **weave security into the very fabric of their software**. This strategic alignment ensures that security considerations are **integral to the software's DNA**.

4. **Developer Awareness and Mitigation**:
   - To meet this requirement, organizations must foster a culture of awareness among **application developers**. These developers need to be well-versed in **API security risks**.
   - Armed with this knowledge, developers can **create and rigorously test code** that effectively **mitigates these risks**. The goal is to build robust software that not only functions seamlessly but also **guards sensitive data** with unwavering vigilance.

PCI DSS underscores the importance of **early security integration**, especially concerning APIs. By weaving security into the very fabric of custom code, organizations can create resilient applications that protect sensitive data from the outset.

### 6.2.2 - Get Your Training On

![Training](/images/training-homoney-football.jpg)

As the son of a football coach, one of the many lessions my father instilled in me was the need to train. Scant weeks after the end of a season, my father and his coaching staff had the players back in the weight room for training. All winter and spring long his team was in the weight room training their muscles to get stronger and be able to endure more. Once school let out, then started "two-a-days" which was morning practice with lunch followed by more practice in the afternoon. This is where all that added power and endurance, so hard won during winter and fall came together. The bonds of brotherhood were forged in the summer as the team trained together. They learned the offensive and defensive playbook until it was second nature and could anticipate each others' action and reactions and in doing so 30+ individuals were forged by the crucible of training into a cohesive and high functioning team. 

So what does this have to do with PCI DSS 4.0? Everything. In section 6.2.2, PCI SSC, rightfully, requires companies to institute a yearly training regimine. That training needs to be:

1. Relevant to their job funtion and languages they code in. 
2. Include secure software design and coding principles
3. Training on the security tools for detecting software vulnerabilities

Remember, that PCI DSS 4.0 includes APIs, so this means that as organization continue to create and expose APIs their developers need to be trained on API Security and the tools used to find and remediate API vulnerabilites. Also, per the good people over at [APIsec University](https://apisecuniversity.com), only 4% of all API testing is focused on security as opposed to functionality.This leaves a huge security gap to fill. 

### 6.2.3 - Secure Software Development: Addressing Vulnerabilities and Best Practices

![Secure Software Development](/images/coding-2.jpg)

In Section 6.2.3, the focus remains on identifying and mitigating vulnerabilities within code. Specifically, it emphasizes the need for thorough reviews of bespoke custom software before its release into production or customer environments. The objective is to proactively identify and rectify potential coding vulnerabilities.

**New and Emerging Vulnerabilities**
Code reviews should extend beyond routine checks. They must actively seek out new and emerging vulnerabilities. Traditionally, these vulnerabilities encompass zero-day exploits or recently discovered security gaps. Notably, such vulnerabilities often relate to third-party libraries and APIs integrated into your applications. To stay vigilant, regularly monitor vulnerability reports and updates.

**Trust No External Data**
When utilizing third-party APIs, a critical best practice is to trust nothing. Your application should never assume that data received from external providers is legitimate. Always scrutinize responses to ensure they align with your expectations. For instance, if your app relies on a third-party API for address normalization, exercise caution. Reject any responses that could be malicious, such as URLs or non-standard address formats.

**Logical Vulnerabilities: A Hidden Threat**
Perhaps the most perilous flaw lies in logical vulnerabilities. These flaws transcend mere code errors; they affect the very logic of your application. When exposed via an API, a logic flaw becomes an open invitation for attackers. To safeguard against this, your custom software must undergo rigorous analysis and testing. Detecting and addressing logic flaws early is paramount.

### Requirement 6.2.4: Safeguarding Custom Software Against Common Attacks
Within Requirement 6, a pivotal section emerges—one that significantly impacts vulnerability testing. Let’s delve into 6.2.4, often regarded as the OWASP (Open Web Application Security Project) segment of this requirement. Its mandate revolves around employing software engineering techniques to prevent or mitigate prevalent software attacks and vulnerabilities in bespoke and custom software.

**Comprehensive Attack Vectors**
This section meticulously outlines various attack vectors that demand consideration. These include:

- Injections
- Authentication Exploits
- Bypassing Authorization
- Cross-Site Scripting (XSS)
- Cross-Site Request Forgery (CSRF)
- Security Misconfiguration
- And more—all aligned with the OWASP Top 10.

**APIs: A Critical Interface**
Explicitly, this section underscores the significance of APIs. When addressing risks, organizations must extend their testing programs beyond web and mobile app interfaces to encompass APIs. These interfaces play a pivotal role in overall security posture.

**Business Logic Attacks**
Building upon concepts introduced earlier, 6.2.4 reinforces the notion of business logic attacks. Beyond understanding how apps are intended to function, organizations must critically assess how these same apps might be abused. Vigilance is key.

**Real-World Example**
Consider an incident where an attacker exploited an API on a crypto trading platform. By manipulating the API, the attacker sold their Ethereum stock as Bitcoin—an ingenious example of a logic flaw.

**API Layer Testing**
While web scanners and penetration testers routinely scrutinize UIs for injection vulnerabilities, it’s imperative to expand this vigilance to the API layer.

## Final Thoughts

PCI DSS 4.0 has many new requirements that are going to change how PCI is thought of. Gone are the days where putting a Web Application Firewall in place was all one needed to alleviate the burden of annual code reviews. The clarion call for security prioritization and training echoes throughout Requirement 6. This is a long overdue revision finally brings PCI DSS into the modern era and takes security seriously.

