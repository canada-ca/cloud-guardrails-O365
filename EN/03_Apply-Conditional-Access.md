# Apply Conditional Access Control Policies

## Objective

Conditional Access is the tool used by Azure Active Directory to bring signals together, to make decisions, and enforce organizational policies. Policies are enforced after the first-factor authentication has been completed.

## Key Considerations

- [ ] Establish Conditional Access Policies (More information is available at <https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/overview>.

Some examples are :

- Any access attempt from outside of the corporate network would either be blocked or require Multifactor Authentication (MFA);
- Any access to the system should be from GC managed devices;
- Any access to the system should be from trusted locations; and
- Any Administrative-level access would require MFA

- [ ] Implement policies to monitor and prevent:
* Risky users
* Risky sign-ins
* Risk detections

- [ ] Implement policies to ensure that trusted devices are used to access the service

## Validation

- [ ] TBD

## References

1. [SPIN 2017-01](https://www.canada.ca/en/treasury-board-secretariat/services/access-information-privacy/security-identity-management/direction-secure-use-commercial-cloud-services-spin.html), subsection 6.2.3
2. CSE Top 10 #3
3. Refer to [CCCS ITSP.30.031 V2 User Authentication Guidance for Information Technology Systems](https://cyber.gc.ca/en/guidance/user-authentication-guidance-information-technology-systems-itsp30031-v3)
4. Refer to the [Guidance on Cloud Authentication for the Government of Canada](https://intranet.canada.ca/wg-tg/cagc-angc-eng.asp)
5. Refer to the [Recommendations for Two-Factor User Authentication Within the Government of Canada Enterprise Domain](https://intranet.canada.ca/wg-tg/rtua-rafu-eng.asp)
6. Related security controls: AC‑2, AC‑2(1), AC‑3, AC‑5, AC‑6, AC‑6(5), AC‑6(10), AC‑7, AC‑9, AC‑19, AC‑20(3), IA‑2, IA‑2(1), IA‑2(2), IA‑2(11), IA‑4, IA‑5, IA‑5(1), IA‑5(6), IA‑5(7), IA‑5(13), IA‑6, IA‑8
