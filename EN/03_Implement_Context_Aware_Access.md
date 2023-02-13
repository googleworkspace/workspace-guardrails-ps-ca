# Implement Context-Aware Access
([Return](/README.md) | [Français](/FR/03_Appliquer-des-politiques-d’accès-contextuelles.md))

## Objective

Using Context-Aware Access, you can create granular access control policies to apps based on attributes such as user identity, location, device security status, and IP address.

[Context-Aware Access](https://support.google.com/a/answer/9275380?hl=en) gives you control over which apps a user can access based on their context, such as whether their device complies with your IT policy.

## Key Considerations

* [ ] Ensure that users understand their responsibilities when using personal devices to access the data and services and the risks of sharing business data with unauthorized users.
* [ ] Establish [Context-Aware access levels](https://support.google.com/a/answer/9262032?hl=en&ref_topic=9262521) that combine conditions and values that define a user or device context. Access levels define the context within which users can access apps based on conditions such as:
  * IP subnet,
  * geographic location,
  * device policy,
  * device OS or
  * create custom access level specifications that meet your specific requirements.
* [ ] Ensure that the established Context-Aware access levels address common access concerns such as:
  * blocking or requiring 2-Step Verification (2SV) for any access attempt from outside of the corporate network;
  * requiring 2-Step Verification for users with administrative roles;
  * requiring 2-Step Verification for Workspace management tasks;
  * blocking or granting access from specific locations;
  * blocking risky sign-in behaviors; and 
  * requiring GC-managed devices for specific applications with consideration of the categorization of the data.
* [ ] Create access levels to the Admin console.
      Avoid a lockout and be sure that at least one admin meets [criteria for access](https://support.google.com/a/answer/10759654).
* [ ] Implement device-based access policies and compliance status to either allow or block access to apps and services.
* [ ] Use the security investigation tool to monitor and run searches related to [Context-Aware Access log events](https://support.google.com/a/answer/9394107?hl=en&ref_topic=9262521), and take action based on the results. 

## Additional Considerations

* [ ] Follow the [best practices for rolling out Context-Aware Access policies](https://support.google.com/a/answer/9275380?hl=en).
* [ ] Consider applying [Context-Aware access with groups](https://support.google.com/a/answer/9668676).
* [ ] Consider applying Context-Aware access levels in [Advanced Mode](https://support.google.com/a/answer/11368990?hl=en&ref_topic=9262521).
* [ ] Ensure access to support in the event of a lockout. If required, follow the steps to [Give users access to the Customer Care Portal](https://support.google.com/a/answer/10759654?hl=en#:~:text=Option%201%3A%20Assign%20the%20Support%20privilege%20to%20an%20existing%20role&text=Click%20the%20role%20that%20you,to%20the%20Customer%20Care%20Portal.).
* [ ] For device-based access:
  * Consider enabling [advanced mobile management](https://support.google.com/a/answer/7396025?hl=en&ref_topic=1734198) to have better control over access to your organization's data.
  * Consider implementing [Data Loss Prevention](https://support.google.com/a/topic/7556687) policies to protect sensitive data and control the apps that can access Google Workspace data.
  * Require additional proof of identity when users sign in to their Google Account with 2-Step Verification (2SV). 
  * Follow the best practices in the [Device management security checklist](https://support.google.com/a/answer/7422256).
  * Consider enforcing access levels based on company ownership or encryption.
  * Consider enforcing access levels based on approval or password status.

## Validation

* [ ] Validate that Context-Aware access levels are in place and meet security requirements.
* [ ] Validate that the access levels established allow for monitoring and preventing risky sign-ins.

## References

1. [Directive on Security Management - Appendix B: Mandatory Procedures for Information Technology Security Control](https://www.tbs-sct.gc.ca/pol/doc-eng.aspx?id=32611&section=procedure&p=B), subsections B.2.3.1, B.2.3.2.4
2. [SPIN 2017-01](https://www.canada.ca/en/treasury-board-secretariat/services/access-information-privacy/security-identity-management/direction-secure-use-commercial-cloud-services-spin.html), subsection 6.2.3
3. CSE Top 10 #3
4. Refer to [CCCS ITSP.30.031 V2 User Authentication Guidance for Information Technology Systems](https://cyber.gc.ca/en/guidance/user-authentication-guidance-information-technology-systems-itsp30031-v3)
5. Refer to the [Guidance on Cloud Authentication for the Government of Canada](https://intranet.canada.ca/wg-tg/cagc-angc-eng.asp)
6. Refer to the [Recommendations for Two-Factor User Authentication Within the Government of Canada Enterprise Domain](https://intranet.canada.ca/wg-tg/rtua-rafu-eng.asp)
7. Related security controls: AC‑2, AC‑2(1), AC‑3, AC‑5, AC‑6, AC‑6(5), AC‑6(10), AC‑7, AC‑9, AC‑19, AC‑20(3), IA‑2, IA‑2(1), IA‑2(2), IA‑2(11), IA‑4, IA‑5, IA‑5(1), IA‑5(6), IA‑5(7), IA‑5(13), IA‑6, IA‑8
   * AU-2, CM-1, CM-2, CM-6, CM-7, SC-20, SC-21
