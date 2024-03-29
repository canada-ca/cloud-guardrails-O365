# Implement Data Protection

([Back](../README.md))

## Objective

Safeguard information and assets hosted in cloud, from unauthorized access, use, disclosure, modification, disposal, transmission, or destruction throughout their life cycle.

## Key Considerations

* Seek guidance from privacy and access to information officials within institutions before storing personal information in cloud-based environments.
* Verify location of service, in accordance with Section 4.4.1.10 of the [Directive on Service and Digital](https://www.tbs-sct.gc.ca/pol/doc-eng.aspx?id=32601)
* Ensure data in transit is encrypted by default (e.g. TLS v1.2, etc.).
* Leverage encryption mechanisms to protect the confidentiality and integrity of data hosted in the cloud service.
* Use CSE-approved cryptographic algorithms and protocols, in accordance with [40.111](https://cyber.gc.ca/en/guidance/cryptographic-algorithms-unclassified-protected-and-protected-b-information-itsp40111) and [40.062](https://www.cse-cst.gc.ca/en/system/files/pdf_documents/itsp.40.062-eng.pdf).
* Enable cloud service level Data Loss Prevention (DLP) policies to allow Exchange Online and SharePoint Online content to be scanned for specific types of data like social security numbers, credit card numbers, or passwords.
* Configure data classification policies to protect internal documents and emails
* Ensure expiration time for external sharing links is set
* Ensure that external users cannot share files, folders, and sites they do not own
* Ensure external file sharing in Teams is enabled for only approved cloud storage services

## Additional Considerations

* Control document sharing by domains with allow list or deny list
* Explore Office 365 Advanced Data Governance for data governance, retention, and expiration (additional licensing required)
* Explore the use of automated DLP with Azure Information Protection for greater consistency and security beyond manual user assignment (additional licensing required)
* Investigate establishment of policies with [Information Barriers (IB)](https://docs.microsoft.com/en-us/microsoftteams/information-barriers-in-teams) to prevent individuals or groups from communicating with each other (additional licensing required)
* Investigate the use of [Compliance Boundaries](https://docs.microsoft.com/en-us/microsoft-365/compliance/set-up-compliance-boundaries?view=o365-worldwide) to create logical boundaries that control the user content locations (such as mailboxes, SharePoint sites, and OneDrive accounts) and support eDiscovery.

## Validation

* TBD

## References

1. [Directive on Security Management - Appendix B: Mandatory Procedures for Information Technology Security Control](https://www.tbs-sct.gc.ca/pol/doc-eng.aspx?id=32611&section=procedure&p=B), subsections B.2.3.4
2. [SPIN 2017-01](https://www.canada.ca/en/treasury-board-secretariat/services/access-information-privacy/security-identity-management/direction-secure-use-commercial-cloud-services-spin.html), subsection 6.2.4
3. Refer to the cryptography guidance in [40.111](https://cyber.gc.ca/en/guidance/cryptographic-algorithms-unclassified-protected-and-protected-b-information-itsp40111) and [40.062](https://www.cse-cst.gc.ca/en/system/files/pdf_documents/itsp.40.062-eng.pdf).
4. Refer to the guidance in [Considerations for Cryptography in Commercial Cloud Services](https://www.canada.ca/en/government/system/digital-government/modern-emerging-technologies/cloud-services/government-canada-consideration-use-cryptography-in-cloud.html).
5. Refer to Section 4.4.1.10 of the [Directive on Service and Digital](https://www.tbs-sct.gc.ca/pol/doc-eng.aspx?id=32601)
6. Related security controls: SC‑8, SC‑8(1), SC‑12, SC‑13, SC‑17, SC‑28, SC‑28(1)
