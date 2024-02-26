# PCI DSS 4, APIs, and You - The Ostrich is Looking Around

![PCI on API Security before 4.0](/images/ostrich-head-in-ground.jpg)

If you hadn't heard the news, the Payment Card Industry (PCI) Security Standards Committee (SSC) Data Security Standards (DSS) have been updated and come into effect on March 31st, 2024. This is a major update that corrects some of the sins of the past and drives home the need to "shift left" with security and also regulates APIs by name. This is a huge difference from the previous PCI DSS standard of 3.2.1, over 50 between the two. Until now PCI DSS was the proverbial Ostrich with it's head buryed. In this post we are going to discuss broadly the changes, specifically in section 6 of PCI DSS 4, and how the PCI SSC has pulled it's head out of the sand in a big way.

## Requirement 6

Requirement 6 of the upcomingnew PCI DSS 4.0 stardard states the following:

> Code repositories that store application code, system configurations, or other configuration data that can
> impact the security of account data or the CDE are in scope for PCI DSS assessments.

This marks the first time that all code repositories are now in-scope for PCI DSS audit and security requirements. Additionally, we would be remiss if we didn't call something out. Throughout Requirement 6 of PCI DSS 4.0 you will oft see repeated the phrase "Bespoke and custom software". The passage pertains to custom code, which can either be internally developed by your organization or supplied by an external party. This code is governed by the requirements set forth in the Data Security Standard (DSS). Specifically, we need to consider the following scenarios:

1. **Account Data Handling**: If the custom software interacts with account data, whether by storing, processing, or transmitting it, it falls squarely within the purview of these DSS requirements. The security of account data is paramount, and any software that touches it must adhere to the stipulated guidelines.
2. **APIs Included**: Notably, this definition extends to Application Programming Interfaces (APIs). Therefore, if your bespoke and tailor-made software integrates APIs—whether for data exchange, communication, or functionality—these APIs are also subject to the same scrutiny.
3. **Holistic Review**: As we delve into the specifics of DSS version 4.0, it’s essential to recognize that the requirements apply not only to the custom-developed applications themselves but also to any APIs they incorporate. In other words, if a particular requirement is relevant to your software, it equally pertains to the APIs woven into its fabric.

What PCI is trying to foster and encourage is a culture of security across the board. No longer is SecOps the sole party responsible for securing all the things. This involves making security fundimental to developments requiring them to implement code testing and review, secure code practices, and remediation before code is released to production. 

With the basics out of the way, let's delve down into PCI DSS 4.0 to see what else pertains to API Security. 

