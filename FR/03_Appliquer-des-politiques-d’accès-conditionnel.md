# Appliquer des politiques d’accès conditionnel

## Objective

Conditional Access is the tool used by Azure Active Directory to bring signals together, to make decisions, and enforce organizational policies. A Conditional Access policy specifies the app or services you want to protect, the conditions under which the apps or services can be accessed, and the users the policy applies to. Policies are enforced after the first-factor authentication has been completed.

## Key Considerations

* [ ] Prevent any unauthorised devices from accessing sensitive business or personal information
* [ ] Ensure that users understand their responsibilities when using personal devices to access the data and services and the risks of sharing business data with unauthorised users
* [ ] Establish [Conditional Access Policies](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/overview) to address common access concerns such as:

- Blocking or requiring Multifactor Authentication (MFA) for any access attempt from outside of the corporate network;
- Requiring multi-factor authentication for users with administrative roles
- Requiring multi-factor authentication for Azure management tasks
- Blocking sign-ins for users attempting to use legacy authentication protocols
- Requiring trusted locations for Azure Multi-Factor Authentication registration
- Blocking or granting access from specific locations 
- Blocking risky sign-in behaviors
- Requiring GC-managed devices for specific applications with consideration of the categorization of the data

* [ ] Implement policies to monitor and prevent:

- Risky users;
- Risky sign-ins; and
- Risk detections

* [ ] Implement device-based conditional access policy and compliance status to either allow or block access to apps and services

## Additional Considerations

* [ ] For **Corporate Owned Devices**, at a minimum, ensure that the following configurations are enforced:
- Allows access to the Web Application Proxy (WAP) and authentication policies to ensure that the device is corporately owned
- Ensure that MFA is enabled for all accounts including use of OTP application

* [ ] For **personal devices**, at a minimum, ensure that the following configurations are enforced:

- Ensure that MFA is enabled for all accounts including use of OTP application
- Configure the data classification capabilities to monitoring and protect sensitive data 
- Configure reverse proxy using [Microsoft Cloud App Security (MCAS)](https://docs.microsoft.com/en-us/cloud-app-security/proxy-intro-aad) to protect data when using web browsers
- Use Intune [Mobile Application Management (MAM)](https://docs.microsoft.com/en-us/mem/intune/apps/mam-faq) to protect data within an application. This includes using MAM and application protection policies on devices not enrolled with Intune Mobile Device Management (MDM). 

## Validation

- [ ] Validate that conditional access policies are in place for devices 
- [ ] Validate that conditional access policies are in place for enabling MFA 

## References

1. [SPIN 2017-01](https://www.canada.ca/en/treasury-board-secretariat/services/access-information-privacy/security-identity-management/direction-secure-use-commercial-cloud-services-spin.html), subsection 6.2.3
2. CSE Top 10 #3
3. Refer to [CCCS ITSP.30.031 V2 User Authentication Guidance for Information Technology Systems](https://cyber.gc.ca/en/guidance/user-authentication-guidance-information-technology-systems-itsp30031-v3)
4. Refer to the [Guidance on Cloud Authentication for the Government of Canada](https://intranet.canada.ca/wg-tg/cagc-angc-eng.asp)
5. Refer to the [Recommendations for Two-Factor User Authentication Within the Government of Canada Enterprise Domain](https://intranet.canada.ca/wg-tg/rtua-rafu-eng.asp)
6. Related security controls: AC‑2, AC‑2(1), AC‑3, AC‑5, AC‑6, AC‑6(5), AC‑6(10), AC‑7, AC‑9, AC‑19, AC‑20(3), IA‑2, IA‑2(1), IA‑2(2), IA‑2(11), IA‑4, IA‑5, IA‑5(1), IA‑5(6), IA‑5(7), IA‑5(13), IA‑6, IA‑8
