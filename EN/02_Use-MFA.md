# Use Multi-Factor Authentication

([Back](../README.md))

## Objective

Multi-factor authentication (MFA) is a method of authentication that requires the use of more than one verification method such as

* Something you know (typically a password);
* Something you have (a trusted device such as a mobile phone);
* Something you are (biometrics);

MFA adds a second layer of security to user sign-ins and transactions. It provides an additional layer of protection to a strong password strategy by providing a way of 'double checking' that you really are the person you are claiming to be when you're using online services. With MFA in place, Office 365 user accounts are still protected against unauthorized access even if a user's password is compromised.

## Key Considerations

* [Implement](https://docs.microsoft.com/en-us/microsoft-365/admin/security-and-compliance/secure-your-business-data?view=o365-worldwide#setup) multi-factor authentication mechanism for external facing interfaces and remote network (cloud) access, in accordance with conditional access policies. The [Recommendations for Two-Factor User Authentication Within the Government of Canada Enterprise Domain](https://intranet.canada.ca/wg-tg/rtua-rafu-eng.asp) recommends, at a minimum, combining:
  * a Level 2 user ID and password with a GC-managed smartphone using either a push notification or an One-time Password (OTP) application; OR
  * a Level 2 user ID and password with an OTP device
* Ensure multifactor authentication is enabled for all users in administrative roles

## Validation

* Confirm that a multi-factor is enabled on the accounts.

## References

1. [Directive on Security Management - Appendix B: Mandatory Procedures for Information Technology Security Control](https://www.tbs-sct.gc.ca/pol/doc-eng.aspx?id=32611&section=procedure&p=B), subsections B.2.3.2.4
2. [SPIN 2017-01](https://www.canada.ca/en/treasury-board-secretariat/services/access-information-privacy/security-identity-management/direction-secure-use-commercial-cloud-services-spin.html), subsection 6.2.3
3. CSE Top 10 #3
4. Refer to [CCCS ITSP.30.031 V2 User Authentication Guidance for Information Technology Systems](https://cyber.gc.ca/en/guidance/user-authentication-guidance-information-technology-systems-itsp30031-v3)
5. Refer to [CCCS ITSAP.30.030 Secure Your Accounts and Devices With Multi-Factor Authentication](https://cyber.gc.ca/en/guidance/secure-your-accounts-and-devices-multi-factor-authentication-itsap30030)
6. Refer to the [Guidance on Cloud Authentication for the Government of Canada](https://intranet.canada.ca/wg-tg/cagc-angc-eng.asp)
7. Refer to the [Recommendations for Two-Factor User Authentication Within the Government of Canada Enterprise Domain](https://intranet.canada.ca/wg-tg/rtua-rafu-eng.asp)
8. Related security controls: AC‑2, AC‑2(1), AC‑3, AC‑5, AC‑6, AC‑6(5), AC‑6(10), AC‑7, AC‑9, AC‑19, AC‑20(3), IA‑2, IA‑2(1), IA‑2(2), IA‑2(11), IA‑4, IA‑5, IA‑5(1), IA‑5(6), IA‑5(7), IA‑5(13), IA‑6, IA‑8
