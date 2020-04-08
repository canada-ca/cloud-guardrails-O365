# Perform Service Hardening

## Objective

Minimize available services and control connectivity by disabling services as well as removing unnecessary accounts from systems. Configure the Office 365 service and the devices from which it is accessed to attempt to filter out and reduce the impact of attempted attacks.

## Key Considerations

* [ ] Configure External collaboration settings
* [ ] Configure Azure Information protection
* [ ] Ensure O365 ATP SafeLinks for Office Applications is Enabled
* [ ] Disable macros where they're not used
* [ ] Disable high-risk macro capabilities
* [ ] Configure macro execution scanning
* [ ] Disable macros unless they are in trusted files - Trusted files (signature or location)
* [ ] Block macros from the Internet
* [ ] Configure [anti-malware protection](https://docs.microsoft.com/en-us/microsoft-365/security/office-365-security/anti-malware-protection?view=o365-worldwide) in the tenant
* [ ] Ensure third party integrated applications are not allowed

### Teams

* [ ] Ensure that users understand the categorization of the Teams site (e.g. Team sites may only be approved for unclassified information)
* [ ] Ensure that users understand their responsibilities for managing information including saving decisions made in the departmental IM repository
* [ ] Owners of team sites are responsible for the management of their Office 365 groups which are the security access control groups that allow access to the team site
* [ ] Ensure you review the Microsoft Apps, Third party Apps and Tenant App that your organization will allow to use within teams
* [ ] Disable external access unless your organization requires collaboration from external users. Configure external access policies to enable collaboration with approved domains.
* [ ] Disable guest access unless is required by your organization. If it is required, establish a guest user access policy and process, and limit the number of guest users where possible. 
* [ ] Disable file sharing services (ShareFile, Dropbox, Box,  Google Drive) if they have not been approved for use in your organization

### Exchange Online

* [ ] Ensure modern authentication for Exchange Online is enabled
* [ ] Ensure calendar details sharing with external users is disabled
* [ ] Configure connection filtering
* [ ] Ensure Exchange Online Spam and Protection Policies are set correctly
* [ ] Ensure the [Common Attachment Types Filter](https://docs.microsoft.com/en-us/exchange/security-and-compliance/mail-flow-rules/common-attachment-blocking-scenarios) is enabled for [malware protection](https://docs.microsoft.com/en-ca/microsoft-365/security/office-365-security/anti-malware-protection?view=o365-worldwide#anti-malware-policies)
* [ ] Ensure mail transport rules [do not forward](https://docs.microsoft.com/en-us/microsoft-365/admin/security-and-compliance/secure-your-business-data?view=o365-worldwide#forwarding) email to external domains
* [ ] Ensure mail transport rules do not whitelist specific domains
* [ ] Ensure that an [anti-phishing policy](https://docs.microsoft.com/en-us/microsoft-365/admin/security-and-compliance/secure-your-business-data?view=o365-worldwide#8-protect-your-email-from-phishing-attacks) has been created
* [ ] Ensure notifications for internal users sending malware is Enabled
* [ ] Ensure the [Advanced Threat Protection Safe Links](https://docs.microsoft.com/en-us/microsoft-365/admin/security-and-compliance/secure-your-business-data?view=o365-worldwide#10-protect-against-phishing-attacks-with-atp-safe-links) policy is enabled
* [ ] Disable unused services per mailbox
* [ ] Configure Transport rule for [ransomware](https://docs.microsoft.com/en-us/microsoft-365/admin/security-and-compliance/secure-your-business-data?view=o365-worldwide#ransomware) to block file extensions that are commonly used for ransomware, or to warn users who receive these attachments in email
* [ ] Authorize all sending IP addresses in Sender Policy Framework (SPF) and ensure that DKIM is enabled for all Exchange Online Domains
* [ ] Apply Domain Keys Identified Mail (DKIM) signatures to all outbound messages for all Exchange Online Domains
* [ ] Establish a minimum Domain-based Message Authentication, Reporting & Conformance (DMARC) policy of “p=none” with at least one address defined as a recipient of aggregate reports, as outlined in CCCS’s Implementation Guidance for Email Domain Protection
* [ ] Add the Canadian Centre for Cyber Security (CCCS) as an aggregate report recipient in the DMARC records. The address that must be included is dmarc@cyber.gc.ca

## Additional Considerations

* [ ] Use [Office Message Encryption](https://docs.microsoft.com/en-us/microsoft-365/admin/security-and-compliance/secure-your-business-data?view=o365-worldwide#7-use-office-message-encryption) to provide protection options when sending mail marked as "Do not forward" or "Encrypt"
* [ ] Consider enabling the [Advanced Threat Protection Safe Attachments](https://docs.microsoft.com/en-us/microsoft-365/admin/security-and-compliance/secure-your-business-data?view=o365-worldwide#9-protect-against-malicious-attachments-and-files-with-atp-safe-attachments) policy
* [ ] Where possible, use automated incident handling and remediation of O365 threats
* [ ] Enable threat intelligence services to assist in the hardening of O365 Advanced Threat Protection
* [ ] Enhance monitoring and control of the cloud environment by using services such as Cloud Access Security Broker (CASB) and User and Entity Behavior Analytics (UEBA) services
* [ ] Ensure product updates and features are reviewed and configured as they become available and where appropriate

## Validation

* [ ] TBD

## References

1. [SPIN 2017-01](https://www.canada.ca/en/treasury-board-secretariat/services/access-information-privacy/security-identity-management/direction-secure-use-commercial-cloud-services-spin.html), subsection 6.2.3
2. CSE Top 10 #3
3. Refer to [CCCS ITSP.30.031 V2 User Authentication Guidance for Information Technology Systems](https://cyber.gc.ca/en/guidance/user-authentication-guidance-information-technology-systems-itsp30031-v3)
4. Refer to the [Guidance on Cloud Authentication for the Government of Canada](https://intranet.canada.ca/wg-tg/cagc-angc-eng.asp)
5. Refer to the [Recommendations for Two-Factor User Authentication Within the Government of Canada Enterprise Domain](https://intranet.canada.ca/wg-tg/rtua-rafu-eng.asp)
6. Related security controls: AC‑2, AC‑2(1), AC‑3, AC‑5, AC‑6, AC‑6(5), AC‑6(10), AC‑7, AC‑9, AC‑19, AC‑20(3), IA‑2, IA‑2(1), IA‑2(2), IA‑2(11), IA‑4, IA‑5, IA‑5(1), IA‑5(6), IA‑5(7), IA‑5(13), IA‑6, IA‑8
