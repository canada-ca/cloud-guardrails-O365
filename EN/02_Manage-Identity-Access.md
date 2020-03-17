# Manage Identity and Access

## Objective

Establish access control policies and procedures for management of administrative privileges. 

## Key Considerations

### Identity

* [ ] Prevent use of Legacy Authentication Protocols
* [ ] Enable Identity Protection 
* [ ] Configure Azure AD Password Protection
* [ ] Configure Federated authentication
* [ ] Configure ADFS to use Azure MFA as the primary authentication mechanism
* [ ] Configure ADFS to Block Legacy Authentication from the Extranet
* [ ] Configure ADFS Web Application Proxy Extranet Lockout
* [ ] When possible, Configure/Prefer Azure AD Smart LockOut to ADFS Web Application Proxy Extranet Lockout"
Configure conditional access using ADFS

### Access

* [ ] Implement a mechanism for uniquely identifying and authenticating organizational users, non-organizational users (if applicable), and processes (for example, username and password)
* [ ] Ensure multifactor authentication is enabled for all users in administrative roles
* [ ] Ensure that between two and four global admins are designated
* [ ] Ensure self-service password reset is enabled
* [ ] Secure administrative roles
* [ ] Enable Privileged Access Management
* [ ] Ensure modern authentication for Exchange Online is enabled
* [ ] Configure password policy in accordance with [GC Password Guidance](https://www.canada.ca/en/government/system/digital-government/password-guidance.html).
* [ ] Configure Office 365 Global Administrator role members
* [ ] Use Non-Global Administrative roles
* [ ] Use dedicated accounts to perform Administrative Tasks
* [ ] Ensure modern authentication for SharePoint applications is required
* [ ] Ensure modern authentication for Skype for Business Online is enabled
* [ ] Minimize number of guest users; add only if needed.

## Additional Considerations

* [ ] Determine access restrictions and configuration requirements for GC-issued endpoint devices, including those of non-privileged and privileged users, and configure access restrictions for endpoint devices accordingly.
* [ ] Control Access to Azure AD administration portal
* [ ] Configure break glass accounts in Azure AD

## Validation

* [ ] Confirm that a privileged account management plan and process has been documented.
* [ ] Confirm password policy aligns with [GC Password Guidance](https://www.canada.ca/en/government/system/digital-government/password-guidance.html) as appropriate.

## References

1. [SPIN 2017-01](https://www.canada.ca/en/treasury-board-secretariat/services/access-information-privacy/security-identity-management/direction-secure-use-commercial-cloud-services-spin.html), subsection 6.2.3
2. CSE Top 10 #3
3. Refer to [CCCS ITSP.30.031 V2 User Authentication Guidance for Information Technology Systems](https://cyber.gc.ca/en/guidance/user-authentication-guidance-information-technology-systems-itsp30031-v3)
4. Refer to the [Guidance on Cloud Authentication for the Government of Canada](https://intranet.canada.ca/wg-tg/cagc-angc-eng.asp)
5. Refer to the [Recommendations for Two-Factor User Authentication Within the Government of Canada Enterprise Domain](https://intranet.canada.ca/wg-tg/rtua-rafu-eng.asp)
6. Related security controls: AC‑2, AC‑2(1), AC‑3, AC‑5, AC‑6, AC‑6(5), AC‑6(10), AC‑7, AC‑9, AC‑19, AC‑20(3), IA‑2, IA‑2(1), IA‑2(2), IA‑2(11), IA‑4, IA‑5, IA‑5(1), IA‑5(6), IA‑5(7), IA‑5(13), IA‑6, IA‑8

