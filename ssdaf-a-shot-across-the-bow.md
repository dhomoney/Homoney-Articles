# The SSDAF - A Shot Across the AppSec Bow

Did you hear that? If you aren't paying attention to the Application Security world, and software in general, you can be excused for not hearing it, but let there be no doubt, the United States Federal government, did just that.

![Shot Across the Bow](/images/shot-across-the-bow.jpg)

The [Secure Software Development Attestation Form (SSDAF)](https://www.cisa.gov/sites/default/files/2024-03/Self-Attestation-Common-Form-03082024-FINAL.pdf) emerged as a significant directive from the United States Federal Government, marking a pivotal moment in the Application Security (AppSec) domain. Released on March 11, 2024, by the [Cybersecurity & Infrastructure Security Agency](https://www.cisa.gov) of the Department of Homeland Security, the SSDAF symbolizes a new and stringent stance on secure software development practices. This move underscores the government's increasing dedication to elevating national cybersecurity standards, an initiative rooted in legislative authority and executive mandates aimed at fortifying the software supply chain against evolving threats.

## Legislative and Executive Foundations

The legal foundation for the SSDAF is anchored in 44 U.S.C. § 3554, alongside the executive guidance provided by [Executive Order 14028](https://www.whitehouse.gov/briefing-room/presidential-actions/2021/05/12/executive-order-on-improving-the-nations-cybersecurity/) titled "Improving the Nation's Cybersecurity." This legislative and executive framework is further bolstered by specific Office of Management and Budget (OMB) Memorandums, which collectively aim to enhance the security measures surrounding the software supply chain. These documents provide the SSDAF with its authority and underscore the government’s commitment to securing software development processes within the broader cybersecurity ecosystem.

## The Purpose of the SSDAF

The primary objective of the SSDAF is to ensure that software procured by the Federal Government is developed with stringent security protocols. This initiative is not just about compliance; it's about assuring the government and, by extension, the national security apparatus that the software it uses is built on a foundation of secure development practices, much like the PCI-DSS standards have done for the payments industry. In certain circumstances, the information collected through the SSDAF could be disclosed to safeguard national security and promote the adoption of enhanced cybersecurity practices across the board. This transparency and accountability mechanism is pivotal in a landscape where software vulnerabilities can have far-reaching implications for national security and public safety.

## Criteria and Process for Attestation

A key aspect of the SSDAF is its requirement for self-attestation by software producers, applicable to software developed or significantly updated after September 14, 2022. This includes products that are continuously updated, reflecting the dynamic nature of software development and the continuous integration/continuous delivery (CI/CD) methodologies that dominate the field. The attestation process mandates that producers of software, excluding software developed by Federal agencies, directly obtained open-source software, third-party components incorporated into end products, or software that is freely obtained and publicly available, confirm their adherence to secure development practices. These practices encompass maintaining secure software development environments, managing a trusted source code supply chain, and employing robust tools for the management of security vulnerabilities.

![Attestation](/images/attestation-cartoon.jpg)

This is where tools, such as Application Security Posture Management(ASPM) come into their own by providing a holistic view of the software supply chain. This holistic view allows ASPMs to quickly provide the lay of the application land and know that secure coding practices are bing adhered to and any security issues are remediated in code before even going to production. The most advanced of these platforms are also integrating runtime intelligence into the mix to give a full code-to-runtime view of the application landscape. That said, almost all ASPM vendors I have reviewed could work on providing more robust reporting that falls in line with major industry standards and government compliance frameworks such as the SSDAF or PCI-DSSv4. 

## The Responsibility of Software Producers

Software producers are tasked with providing comprehensive information regarding their development practices and the measures in place to ensure the security of their software. This includes a declaration of the steps taken to mitigate risks associated with the use of third-party components, a concern that has gained prominence given the complex ecosystems of dependencies that modern software applications often rely on, the log4j and OpenSSL vulnerabilities being recent examples. The form must be endorsed by the company’s CEO or an authorized representative, signifying a top-down commitment to secure software development. Alternatively, producers can opt to submit an assessment conducted by an approved third-party assessor, offering flexibility in demonstrating compliance with the outlined security practices.

## Implications and the Shift in AppSec Paradigms

The introduction of the SSDAF represents a sea change in the approach to software security, catalyzing a shift towards more proactive and preventive measures in software development. As digital transformation and the integration of artificial intelligence continue to redefine the technological landscape, the importance of securing the software supply chain has never been more apparent. The SSDAF encourages organizations to embrace a "shift left" approach, integrating security considerations early in the software development lifecycle, thereby alleviating the pressure on SecOps teams to secure applications post-deployment, a near impossibility in modern CI/CD environments.

This paradigm shift also places a renewed emphasis on equipping developers with tools that enhance, rather than obfuscate, the identification and remediation of security issues such as ASPM. The clutter and noise often associated with traditional security tools can obscure critical vulnerabilities, necessitating a more refined toolset that prioritizes clarity and precision in vulnerability detection. ASPM's ability to bring clarity and filter out the noise allows developers to focus on actual threats instead of chasing false positives.

## Broader Implications for the Business Sector

Perhaps most significantly, the SSDAF extends accountability beyond the traditional confines of IT and security departments, implicating the broader business landscape in the quest for secure software. In an era where the consequences of security failures can extend to congressional hearings and public scrutiny, the responsibility for delivering secure code no longer rests solely on the shoulders of CIOs and CISOs, or the SecOps engineers in the trenches. This regulatory move underlines the reality that businesses, as a whole, bear the consequences of cybersecurity lapses, highlighting the necessity for a collective and informed effort to elevate software security standards.

![Grilled by Congress](/images/cartoon-congressional-inquiry.jpg)

In conclusion, the SSDAF is not merely a regulatory formality; it is a clarion call to the software development and cybersecurity communities. It demands a reevaluation of current practices and a unified move towards embedding security into the DNA of software development. As we navigate the complexities of modern software creation and deployment, the principles encapsulated in the SSDAF serve as guiding lights toward a more secure and resilient digital future.

There is a lot more to say on this an the Application Security world in general. Reach out and let's discuss during an [Application Security Briefing](https://www.wwt.com/briefing/application-security-briefing)
