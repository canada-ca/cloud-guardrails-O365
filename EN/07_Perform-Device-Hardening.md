# Perform Device Hardening

## Objective

The security posture of the devices being used to access the service should be considered. As a minimum, organisations need to ensure that devices are fully patched, are not using administrative privileges, have malware defences in place and are collecting security logs.

## Key Considerations

* [ ] Prevent any unauthorised devices from accessing sensitive business or personal information.
* [ ] Use GC managed endpoints and validate that the device is compliant such as requiring a minimum, and supported, operating system version
* [ ] As per the [ITPIN 2018-03](https://www.canada.ca/en/government/system/digital-government/modern-emerging-technologies/policy-implementation-notices/direction-windows10-desktop-operating-system-migration-configuration.html), when using Windows 10 devices, the Windows 10 GC Minimum version and configuration as specified on the [GC Windows 10 Configuration Baseline](https://gcconnex.gc.ca/groups/profile/12903340/wtd-common-desktop-operating-environment-environnement-dexploitation-commun-des-ordinateurs-de-bureau-des-atmt?language=en#20998653) (accessible only on the Government of Canada network) page must be implemented. The GC Minimum configuration standard prescribes Windows 10 configuration standards which are necessary to maintain the security of GC networks and workplace technology devices.

### Mobile Device Management

* [ ] Ensure mobile device management polices are set to require advanced security configurations to protect from basic internet attacks
* [ ] Ensure mobile devices require the use of a password
* [ ] Configure mobile device password policy is configured, in accordance with [GC Password Guidance](https://www.canada.ca/en/government/system/digital-government/password-guidance.html).
* [ ] Ensure that users cannot connect from devices that are jail broken or rooted
* [ ] Configure settings to lock multiple devices after a period of inactivity to prevent unauthorized access
* [ ] Ensure that mobile device encryption is enabled to prevent unauthorized access to mobile data
* [ ] Ensure that devices connecting have AV and a local firewall enabled
* [ ] Ensure mobile device management policies are required for email profiles

## Validation

* [ ] TBD

## References

1. [Directive on Security Management - Appendix B: Mandatory Procedures for Information Technology Security Control](https://www.tbs-sct.gc.ca/pol/doc-eng.aspx?id=32611&section=procedure&p=B), subsections B.2.3.1, B.2.3.3.3, B.2.3.4
2. [SPIN 2017-01](https://www.canada.ca/en/treasury-board-secretariat/services/access-information-privacy/security-identity-management/direction-secure-use-commercial-cloud-services-spin.html)
3. CSE Top 10
4. Refer to [CCCS ITSP.30.031 V2 User Authentication Guidance for Information Technology Systems](https://cyber.gc.ca/en/guidance/user-authentication-guidance-information-technology-systems-itsp30031-v3)
5. Refer to the [GC Password Guidance](https://www.canada.ca/en/government/system/digital-government/password-guidance.html)
6. Refer to the [ITPIN 2018-03](https://www.canada.ca/en/government/system/digital-government/modern-emerging-technologies/policy-implementation-notices/direction-windows10-desktop-operating-system-migration-configuration.html)
