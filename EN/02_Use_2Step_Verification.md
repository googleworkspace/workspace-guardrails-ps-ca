# Use 2-Step Verification
([Return](/README.md) | [Français](/FR/02_Utiliser-2SV.md))

## Objective

2-Step Verification puts an extra barrier between your business and cybercriminals who try to steal usernames and passwords to access business data. Turning on 2-Step Verification is the single most important action you can take to protect your business.

With 2-Step Verification, your users sign in to their account in two steps with something they know (their password) and something they have (their phone or a  Security Key).

When you set up 2-Step Verification, you choose the second verification step for your users.
* [ ] Security keys
* [ ] Google prompt
* [ ] Google Authenticator and other verification code generators
* [ ] Backup codes
* [ ] Text message or phone call

## Key Considerations

* [ ] [Enforce 2-Step Verification](https://support.google.com/a/answer/175197?hl=en&ref_topic=2759193) for administrators and key users.
* [ ] Consider using security keys or alternatives such as Google prompt or Google authenticator. The [Recommendations for Two-Factor User Authentication Within the Government of Canada Enterprise Domain](https://intranet.canada.ca/wg-tg/rtua-rafu-eng.asp) recommends, at a minimum, combining:
  * a Level 2 user ID and password with a GC-managed smartphone using either a push notification or an One-time Password (OTP) application; OR
  * a Level 2 user ID and password with an OTP device

If using a third-party identity provider:
* [ ] If you’re using a third-party IdP to authenticate users for accessing Google products and SSO is enabled for your top-level organization, by default Google's 2-Step Verification doesn't apply when users sign in through that SSO service.
Note: You can set a policy to allow additional risk-based authentication challenges and 2-Step Verification (2SV) (if configured). 
* [ ] Super administrators don't use SSO when signing in to their administrator accounts. If they’re enrolled in 2SV, they must provide a second authentication factor when they sign in.

## Validation

* [ ] Confirm that 2-Step Verification is enabled on the accounts.

## References

1. [Directive on Security Management - Appendix B: Mandatory Procedures for Information Technology Security Control](https://www.tbs-sct.gc.ca/pol/doc-eng.aspx?id=32611&section=procedure&p=B), subsections B.2.3.2.4
2. [SPIN 2017-01](https://www.canada.ca/en/treasury-board-secretariat/services/access-information-privacy/security-identity-management/direction-secure-use-commercial-cloud-services-spin.html), subsection 6.2.3
3. CSE Top 10 #3
4. Refer to [CCCS ITSP.30.031 V2 User Authentication Guidance for Information Technology Systems](https://cyber.gc.ca/en/guidance/user-authentication-guidance-information-technology-systems-itsp30031-v3)
5. Refer to [CCCS ITSAP.30.030 Secure Your Accounts and Devices With Multi-Factor Authentication](https://cyber.gc.ca/en/guidance/secure-your-accounts-and-devices-multi-factor-authentication-itsap30030)
6. Refer to the [Guidance on Cloud Authentication for the Government of Canada](https://intranet.canada.ca/wg-tg/cagc-angc-eng.asp)
7. Refer to the [Recommendations for Two-Factor User Authentication Within the Government of Canada Enterprise Domain](https://intranet.canada.ca/wg-tg/rtua-rafu-eng.asp)
8. Related security controls: AC‑2, AC‑2(1), AC‑3, AC‑5, AC‑6, AC‑6(5), AC‑6(10), AC‑7, AC‑9, AC‑19, AC‑20(3), IA‑2, IA‑2(1), IA‑2(2), IA‑2(11), IA‑4, IA‑5, IA‑5(1), IA‑5(6), IA‑5(7), IA‑5(13), IA‑6, IA‑8
   * AU-2, CM-1, CM-2, CM-6, CM-7, SC-20, SC-21
