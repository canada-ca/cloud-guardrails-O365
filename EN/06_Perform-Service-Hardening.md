# Perform Service Hardening

## Objective

TBD

## Key Considerations

* [ ] Configuring  External collaboration settings
* [ ] Configure Azure Information protection
* [ ] Ensure O365 ATP SafeLinks for Office Applications is Enabled
* [ ] Disable macros where they're not used
* [ ] Disable high-risk macro capabilities
* [ ] Configure macro execution scanning
* [ ] Disable macros unless they are in trusted files - Trusted files (signature or location)
* [ ] Block macros from the Internet
* [ ] Configure anti-malware protection in your tenant

### Exchange Online

* [ ] Ensure modern authentication for Exchange Online is enabled
* [ ] Ensure the Common Attachment Types Filter is enabled
* [ ] Ensure mail transport rules do not forward email to external domains
* [ ] Ensure mail transport rules do not whitelist specific domains
* [ ] Ensure that an anti-phishing policy has been created
* [ ] Ensure that DKIM is enabled for all Exchange Online Domains
* [ ] Ensure that SPF records are published for all Exchange Domains
* [ ] Ensure DMARC Records for all Exchange Online domains are published
* [ ] Ensure notifications for internal users sending malware is Enabled
* [ ] Ensure the Advanced Threat Protection Safe Links policy is enabled
* [ ] Disable unused services per mailbox
* [ ] Configure Transport rule for ransomware

## Validation

* [ ] TBD

## References

1. [SPIN 2017-01](https://www.canada.ca/en/treasury-board-secretariat/services/access-information-privacy/security-identity-management/direction-secure-use-commercial-cloud-services-spin.html), subsection 6.2.3
2. CSE Top 10 #3
3. Refer to [CCCS ITSP.30.031 V2 User Authentication Guidance for Information Technology Systems](https://cyber.gc.ca/en/guidance/user-authentication-guidance-information-technology-systems-itsp30031-v3)
4. Refer to the [Guidance on Cloud Authentication for the Government of Canada](https://intranet.canada.ca/wg-tg/cagc-angc-eng.asp)
5. Refer to the [Recommendations for Two-Factor User Authentication Within the Government of Canada Enterprise Domain](https://intranet.canada.ca/wg-tg/rtua-rafu-eng.asp)
6. Related security controls: AC‑2, AC‑2(1), AC‑3, AC‑5, AC‑6, AC‑6(5), AC‑6(10), AC‑7, AC‑9, AC‑19, AC‑20(3), IA‑2, IA‑2(1), IA‑2(2), IA‑2(11), IA‑4, IA‑5, IA‑5(1), IA‑5(6), IA‑5(7), IA‑5(13), IA‑6, IA‑8

