# Manage Identity and Access
([Return](/README.md) | [Français](/FR/01_Gérer-l’identité-et-l’accès.md))

## Objective

Manage identities and establish access control policies and procedures for management of administrative privileges.

## Key Considerations

### Identity

* [ ] Add Cloud Identity to Google Workspace to manage identities.
* [ ] Configure controls to protect passwords in accordance with the [Implementation Strategy for GC Password Guidance](https://www.gcpedia.gc.ca/gcwiki/images/c/c0/Implementation_Strategy_for_GC_Password_Guidance.pdf) (accessible only on the Government of Canada network).
* [ ] Configure break glass (super admin) accounts in Google Workspace.
* [ ] Ensure that between two and four super admins are designated.
* [ ] Enable Password Alert to make sure users don't use their corporate passwords on other sites.
* [ ] Follow Google's [security best practices for administrator accounts](https://support.google.com/a/answer/9011373).

If using a third-party identity provider consider the following best practices for your Google Workspace configuration:

* [ ] Maintain strong passwords for Google Workspace accounts. These passwords are less likely to be used, so they may represent an attack surface.
* [ ] Enable Single Sign-On and ensure that your IdP and all systems it depends on are configured securely.
* [ ] Follow Google's [best practices for federating Google Cloud with an external identity provider](https://cloud.google.com/architecture/identity/best-practices-for-federating).

### Access

* [ ] Implement a mechanism for uniquely identifying and authenticating organizational users, non-organizational users (if applicable), and processes (for example, username and password).
* [ ] Require 2-Step Verification for users.
* [ ] Ensure login challenges have been set up for suspicious login attempts.
* [ ] Enforce security keys or other physical authentication device, at least for admins and other high-value accounts.
* [ ] Enforce password policy in accordance with [GC Password Guidance](https://www.canada.ca/en/government/system/digital-government/password-guidance.html).
* [ ] Implement role-based access and use roles with least privileges where possible (e.g. use non-global administrative roles).
* [ ] Use dedicated accounts to perform Administrative Tasks.
* [ ] Control who can access the Admin portal, Google Workspace and Google services.
* [ ] Disallow access to apps that are less secure.
* [ ] Block access to consumer accounts.
* [ ] Regularly review security reports and alerts, in accordance with the [Enable logging and monitoring](04_Enable-Logging-and-Monitoring.md) guardrail.
* [ ] Maintain your security after an employee leaves by completing the following [best practices](https://support.google.com/a/answer/6329207?hl=en&ref_topic=7558661).

## Additional Considerations

* [ ] Require external collaborators to sign in with a Google Account. If they don't have a Google Account, they can create one at no cost. 
* [ ] Consider enabling the [Advanced Protection Program](https://support.google.com/a/answer/9378686?hl=en) to protect Google accounts against targeted online attacks.
* [ ] Determine access restrictions and configuration requirements for GC-issued endpoint devices, including those of non-privileged and privileged users, and configure access restrictions accordingly
* [ ] Ensure that Google session control is configured

If using Azure Active Directory/O365:
* [ ] Prevent the use of Legacy Authentication Protocols.
* [ ] Consider enabling Identity Protection (additional licensing required)
* [ ] Consider controlling administrative tasks with privileged access management (additional licensing required)
* [ ] Investigate just-in-time access to enable administrative access on an as an when required basis (additional licensing required)

## Validation

* [ ] Confirm that a privileged account management plan and process has been documented.
* [ ] Confirm password policy aligns with [GC Password Guidance](https://www.canada.ca/en/government/system/digital-government/password-guidance.html) (accessible only on the Government of Canada network) as appropriate.

## References

1. [Directive on Security Management - Appendix B: Mandatory Procedures for Information Technology Security Control](https://www.tbs-sct.gc.ca/pol/doc-eng.aspx?id=32611&section=procedure&p=B), subsections B.2.3.1, B.2.3.2.4
2. [SPIN 2017-01](https://www.canada.ca/en/treasury-board-secretariat/services/access-information-privacy/security-identity-management/direction-secure-use-commercial-cloud-services-spin.html), subsection 6.2.3
3. CSE Top 10 #3
4. Refer to [CCCS ITSP.30.031 V2 User Authentication Guidance for Information Technology Systems](https://cyber.gc.ca/en/guidance/user-authentication-guidance-information-technology-systems-itsp30031-v3)
5. Refer to the [Guidance on Cloud Authentication for the Government of Canada](https://intranet.canada.ca/wg-tg/cagc-angc-eng.asp) (accessible only on the Government of Canada network)
6. Refer to the [Recommendations for Two-Factor User Authentication Within the Government of Canada Enterprise Domain](https://intranet.canada.ca/wg-tg/rtua-rafu-eng.asp) (accessible only on the Government of Canada network)
7. Related security controls: AC‑2, AC‑2(1), AC‑3, AC‑5, AC‑6, AC‑6(5), AC‑6(10), AC‑7, AC‑9, AC‑19, AC‑20(3), IA‑2, IA‑2(1), IA‑2(2), IA‑2(11), IA‑4, IA‑5, IA‑5(1), IA‑5(6), IA‑5(7), IA‑5(13), IA‑6, IA‑8
   * AU-2, CM-1, CM-2, CM-6, CM-7, SC-20, SC-21
