# Perform Device Hardening
([Return](/README.md) | [Français](/FR/07_Exécuter-le-renforcement-des-appareils.md))

## Objective

The security posture of the devices being used to access the service should be considered. As a minimum, organizations need to ensure that devices are fully patched, are not using administrative privileges, have malware defences in place and are collecting security logs.

As an administrator, you can help protect work data on users’ personal devices (BYOD) and on your organization’s company-owned devices by using Google endpoint management features and settings. Other security features provide stronger account protection, granular access control, and data protection.

## Key Considerations

* [ ] Prevent any unauthorized devices from accessing sensitive business or personal information.
* [ ] Use GC managed endpoints and validate that the device is compliant such as requiring a minimum, and supported, operating system version.
* [ ] As per the [ITPIN 2018-03](https://www.canada.ca/en/government/system/digital-government/modern-emerging-technologies/policy-implementation-notices/direction-windows10-desktop-operating-system-migration-configuration.html), when using Windows 10 devices, the Windows 10 GC Minimum version and configuration as specified on the [GC Windows 10 Configuration Baseline](https://gcconnex.gc.ca/groups/profile/12903340/wtd-common-desktop-operating-environment-environnement-dexploitation-commun-des-ordinateurs-de-bureau-des-atmt?language=en#20998653) (accessible only on the Government of Canada network) page must be implemented. The GC Minimum configuration standard prescribes Windows 10 configuration standards which are necessary to maintain the security of GC networks and workplace technology devices.
* [ ] Define rules to automate device management tasks and get security alerts.
* [ ] Ensure you follow the guidelines established for [Google endpoint managament](https://support.google.com/a/topic/24642?hl=en&ref_topic=10012113).

### Mobile Device Management

* [ ] Ensure mobile device management polices are set to require advanced security configurations to protect from basic internet attacks
* [ ] Ensure mobile devices require the use of a password
* [ ] Ensure mobile device password policy is configured, in accordance with [GC Password Guidance](https://www.canada.ca/en/government/system/digital-government/password-guidance.html).
* [ ] Block compromised devices
* [ ] Lock down or wipe corporate data from missing devices
* [ ] Manage Android/iOS apps used for work
* [ ] Require device encryption
* [ ] Apply device restrictions
* [ ] Automatically block mobile devices that don't comply with your policies
* [ ] Block potentially dangerous mobile apps

### Computers that access work data

* [ ] Turn on endpoint verification
* [ ] Restrict Google Drive for desktop to company-owned devices
* [ ] Set up Google Credential Provider for Windows (GCPW) to let users sign in to Windows 10 computers with their work Google Account (if applicable)
* [ ] Restrict user privileges on company-owned Windows computers

### More security considerations for all devices

* [ ] Prevent unauthorized access to a user's account
* [ ] Use Context-Aware Access to conditionally allow access to Google apps
* [ ] Identify sensitive data in Google Drive, Docs, Sheets, Slides and Gmail

## Validation

* [ ] Validate that device restrictions are in place
* [ ] Validate that device encryption is turned on
* [ ] Validate that iOS and Android apps are being managed
* [ ] Validate that endpoint verification is enabled

## References

1. [Directive on Security Management - Appendix B: Mandatory Procedures for Information Technology Security Control](https://www.tbs-sct.gc.ca/pol/doc-eng.aspx?id=32611&section=procedure&p=B), subsections B.2.3.1, B.2.3.3.3, B.2.3.4
2. [SPIN 2017-01](https://www.canada.ca/en/treasury-board-secretariat/services/access-information-privacy/security-identity-management/direction-secure-use-commercial-cloud-services-spin.html)
3. CSE Top 10
4. Refer to [CCCS ITSP.30.031 V2 User Authentication Guidance for Information Technology Systems](https://cyber.gc.ca/en/guidance/user-authentication-guidance-information-technology-systems-itsp30031-v3)
5. Refer to the [GC Password Guidance](https://www.canada.ca/en/government/system/digital-government/password-guidance.html)
6. Refer to the [ITPIN 2018-03](https://www.canada.ca/en/government/system/digital-government/modern-emerging-technologies/policy-implementation-notices/direction-windows10-desktop-operating-system-migration-configuration.html)
