# Manage Administrative Access

## Objective

Establish access control policies and procedures for management of administrative privileges. 

## Key Considerations

* [ ] Implement a mechanism for uniquely identifying and authenticating organizational users, non-organizational users (if applicable), and processes (for example, username and password).
* [ ] Prevent use of Legacy Authentication Protocols
* [ ] Ensure multifactor authentication is enabled for all users in administrative roles
* [ ] Ensure that between two and four global admins are designated
* [ ] Ensure the Azure AD 'Risky sign-ins' report is reviewed at least weekly
* [ ] Where possible, enable administrative access for administrators in a time-boxed and just-in-time manner (using Azure AD Privileged Identity Manager)
* [ ] External access (if this is permitted) will require the use of MFA through Azure AD Conditional Access.
* [ ] Minimize number of guest users; add only if needed.
* [ ] Change default passwords.
* [ ] Configure password policy in accordance with [GC Password Guidance](https://www.canada.ca/en/government/system/digital-government/password-guidance.html).
* [ ] Ensure self-service password reset is enabled
* [ ] Determine access restrictions and configuration requirements for GC-issued endpoint devices, including those of non-privileged and privileged users, and configure access restrictions for endpoint devices accordingly.
* [ ] Ensure third party integrated applications are not allowed
* [ ] Control access to Azure AD administration portal

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

