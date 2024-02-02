# ASPM and API Security: Complementarity at its Finest

![Complementarity](/images/complementarity.jpg)

Complementarity is a word not often heard outside Quantum Physics circles these days, but its more traditional use here I think is more aprapos here than the meaning used by Quantum Physics. If you look it up there are a bunch of variations, but the [Cambridge Dictionary](https://dictionary.cambridge.org/us/dictionary/english/complementarity) says it best

complementarity
: the quality of being different but useful when combined

This, I think, is a great definition to use for the relationship between Application Security Posture Management (ASPM) and API security, and especially between [Akamai](https://www.wwt.com/partner/akamai/overview) and [Apiiro](https://apiiro.com) and the complementarity of their runtime API security offering and ASPM. These two come at API Security from different, but very complementary ways. Akamai's API Security staunchly in the Defend side of security while Apiiro takes a Secure side approach, protecting the software supply-chain. 

## Complete code-to-runtime API discovery

One of the very core tenants of API Security is discovery, for you cannot secure that which you don't know about. This has long been an Achille's heal of API Security. There have been multiple differing attempts, varying from crawlers to forcing traffic rerouted through SaaS-only solutions, and these work to varying degrees, but all have flaws. Crawlers, to date, miss too much and still having the issue of having to know where to crawl for your APIs. The forcing traffic through an SaaS, is a bit better in that all external internet facing traffic would pass through and this detection is typically more accurate, but this has its own issues, such as the effort and disruption of doing this, if you aren't using a SaaS CDN already, and you still will not catch or detect potential B2B APIs that run over private links or APIs placed in the Cloud in places the SecOps team is unaware of. This is where the addition of Apiiro to the mix closes the loop, by connecting to the repositories themselves.  

Using deep code analysis, Apiiro continuously inventories all APIs and data models. It audits all activity in repositories to detect new and significant changes to APIs and identify vulnerabilities before they are committed or deployed. Apiiro is powered by our Risk Graph, which can also highlight APIs connected to sensitive data (such as PII, PCI, PHI) or other security weaknesses.

This level of visibility into the code allows for the discovery of API components that may be vulnerable to misconfigurations, code logic flaws, design flaws, and common coding errors. It is a valuable addition to runtime API security.

Having visibility into the code-to-runtime helps in discovering shadow APIs and enables developers to prevent API weaknesses from being deployed. This saves time that would otherwise be spent on reactive risk mitigation. Apiiro's proactive approach also helps modernize risk assessment processes and triggers security reviews based on risky material API changes in the code.

## Prioritization of API risks in code with runtime context from Akamai 

The level of risk that an API weakness in code poses to your organization depends on the likelihood and impact of that risk. For instance, a risk in a publicly exposed API is more likely to become a real risk, and an API that handles sensitive data has a greater potential impact on your business.

By combining Apiiro's deep contextual knowledge of code with Akamai API Security's insight into API behavior and threats at runtime, customers can accurately assess the likelihood and impact of a risk, and prioritize API risks critical to the business.

![Filtered Risk Pane](/images/filtered-risk-pane.jpg)

Fusing code and runtime context enables teams to prioritize business-critical API security issues, reduce false positives, and save time triaging backlogs and fixing risks. 

## Visibility into API security coverage and gaps

It can often be a daunting task for Application Security (AppSec) teams, particularly those operating within large organizations, to have complete visibility into the extent and effectiveness of security testing efforts. This lack of clarity can hinder their ability to assess the overall security posture of their applications. However, with the help of Apiiro's ASPM solution and comprehensive deep code analysis, offers a compelling solution. ASPM empowers AppSec teams to holisticly view security testing coverage, including from external sources such as Akamai API Security and not just from within their own code repositories. By consolidating and analyzing security testing data from various sources, ASPM empowers organizations to make informed decisions and effectively address any potential vulnerabilities or weaknesses in their applications.

![Security Coverage](/images/security-coverage.jpg)

That coverage mapping, tied to Apiiro’s code-based insights (i.e., handling of sensitive data, amount of risky changes), can help dictate where security testing should be done and where gaps exist. For example, you may want to ensure that all high business impact (HBI) applications or repositories containing APIs and sensitive data—which you can surface using Apiiro’s Risk Graph Explorer, as seen below—are covered by Akamai. 

![Risk Graph Explorer Enriched by Akamai](/images/risk-graph-explorer.jpg)

Ultimately, this insight has the ability to minimize API security testing gaps and ensure more complete coverage.

## Unifying API risk management from code to runtime

The integration between Akamai API Security and Apiiro ASPM enables teams to finally have comprehensive API discovery, testing, prioritization, and remediation with continuous and complete visibility of APIs and API risks from development to runtime. This integration is the first step in providing an integrated view of API risks that unifies code and runtime insights, thus allowing SecOps to proactively secure their APIs and efficiently prioritize and remediate API risks. 

In the end, this is exciting news for DevSecOps all around and closes some major loopholes in API Security and ties in ASPM to the Defend side for real security, from code to runtime. 