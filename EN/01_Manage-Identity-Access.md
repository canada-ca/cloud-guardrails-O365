# Manage Identity and Access

## Objective

Manage identities and establish access control policies and procedures for management of administrative privileges.

## Key Considerations

### Identity

* [ ] Prevent use of Legacy Authentication Protocols
* [ ] Configure Azure AD Password Protection in accordance with the [Implementation Strategy for GC Password Guidance](https://www.gcpedia.gc.ca/gcwiki/images/c/c0/Implementation_Strategy_for_GC_Password_Guidance.pdf) (*_accessible only on the Government of Canada network_*)
* [ ] Configure break glass accounts in Azure AD
* [ ] Leverage Federated authentication where available

If using ADFS, consider the following:

* [ ] Configure ADFS to use Azure MFA as the primary authentication mechanism
* [ ] Configure ADFS to Block Legacy Authentication from the Extranet
* [ ] Configure ADFS Web Application Proxy Extranet Lockout
* [ ] Install  trusted certificate on the ADFS server
* [ ] Implement additional security settings in ADFS to mitigate man-in-the-middle attacks

### Access

* [ ] Implement a mechanism for uniquely identifying and authenticating organizational users, non-organizational users (if applicable), and processes (for example, username and password)
* [ ] Ensure multifactor authentication is enabled for all users in administrative roles
* [ ] Ensure that between two and four global admins are designated
* [ ] Implement role-based access and use roles with least privileges where possible (e.g. use non-global administrative roles)
* [ ] Configure Office 365 Global Administrator role members
* [ ] Use dedicated accounts to perform Administrative Tasks
* [ ] Control Access to Azure AD administration portal
* [ ] Ensure modern authentication for SharePoint applications is required
* [ ] Ensure modern authentication for Teams (formerly Skype for Business Online) is enabled
* [ ] Ensure modern authentication for Exchange Online is enabled
* [ ] Configure password policy in accordance with [GC Password Guidance](https://www.canada.ca/en/government/system/digital-government/password-guidance.html).
* [ ] Disable guest user access by default. Add only the minimum number of accounts, if needed, in conformance to an approved guest user policy and procedures including ensuring that a [secure sharing environment](https://docs.microsoft.com/en-us/microsoft-365/solutions/create-secure-guest-sharing-environment?view=o365-worldwide) has been established.
* [ ] Regularly review reports for all administrative accounts and access reports, in accordance with the [Enable logging and monitoring](04_Enable-Logging-and-Monitoring.md) guardrail

## Additional Considerations

* [ ] Consider enabling Identity Protection (additional licensing required)
* [ ] Consider controlling administrative tasks with privileged access management (additional licensing required)
* [ ] Investigate just-in-time access to enable administrative access on an as an when required basis (additional licensing required)
* [ ] Limit disclosure of sensitive GC information to support personnel. If access to data is required, leverage the customer lockbox feature (additional licensing required)
* [ ] Determine access restrictions and configuration requirements for GC-issued endpoint devices, including those of non-privileged and privileged users, and configure access restrictions accordingly

## Validation

* [ ] Confirm that a privileged account management plan and process has been documented.
* [ ] Confirm password policy aligns with [GC Password Guidance](https://www.canada.ca/en/government/system/digital-government/password-guidance.html) *_(accessible only on the Government of Canada network)_* as appropriate.

## References

1. [Directive on Security Management - Appendix B: Mandatory Procedures for Information Technology Security Control](https://www.tbs-sct.gc.ca/pol/doc-eng.aspx?id=32611&section=procedure&p=B), subsections B.2.3.1, B.2.3.2.4
2. [SPIN 2017-01](https://www.canada.ca/en/treasury-board-secretariat/services/access-information-privacy/security-identity-management/direction-secure-use-commercial-cloud-services-spin.html), subsection 6.2.3
3. CSE Top 10 #3
4. Refer to [CCCS ITSP.30.031 V2 User Authentication Guidance for Information Technology Systems](https://cyber.gc.ca/en/guidance/user-authentication-guidance-information-technology-systems-itsp30031-v3)
5. Refer to the [Guidance on Cloud Authentication for the Government of Canada](https://intranet.canada.ca/wg-tg/cagc-angc-eng.asp) *_(accessible only on the Government of Canada network)_*
6. Refer to the [Recommendations for Two-Factor User Authentication Within the Government of Canada Enterprise Domain](https://intranet.canada.ca/wg-tg/rtua-rafu-eng.asp) *_(accessible only on the Government of Canada network)_*
7. Related security controls: AC‑2, AC‑2(1), AC‑3, AC‑5, AC‑6, AC‑6(5), AC‑6(10), AC‑7, AC‑9, AC‑19, AC‑20(3), IA‑2, IA‑2(1), IA‑2(2), IA‑2(11), IA‑4, IA‑5, IA‑5(1), IA‑5(6), IA‑5(7), IA‑5(13), IA‑6, IA‑8
