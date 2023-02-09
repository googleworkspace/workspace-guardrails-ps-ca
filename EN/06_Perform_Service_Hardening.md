# Perform Service Hardening
([Return](/README.md) | [Français](/FR/06_Exécuter-le-renforcement-des-services.md))

## Objective

Minimize available services and control connectivity by disabling services as well as removing unnecessary accounts from systems. Configure Google Workspace and the devices from which it is accessed to strengthen the security and privacy of company data.

Implementation guidance is provided in the [Security checklist](https://support.google.com/a/answer/7587183)

## Key Considerations

### Apps 

* [ ] Review third-party app access to core services
* [ ] Block access to less secure apps
* [ ] Create a list of trusted apps
* [ ] Control access to Google core services

### Calendar

* [ ] Limit external calendar sharing
* [ ] Warn users when they invite external guests

### Google Chat

* [ ] Limit who can chat externally
* [ ] Warn users when chatting outside their domain
* [ ] Set a chat invitation policy
* [ ] Define and implement DLP rules to protect sensitive data in messages and files in Google Chat

### Chrome browser or Chrome OS devices

* [ ] Keep Chrome browser or Chrome OS updated
* [ ] Set basic Chrome OS device and Chrome browser policies
* [ ] Set advanced Chrome browser policies
* [ ] Set a Windows desktop browser policy

### Drive

* [ ] Set sharing options for your domain
* [ ] Set the default for link sharing
* [ ] Warn users when they share a file outside your domain
* [ ] Limit file access to recipients only
* [ ] Prevent users from publishing on the web
* [ ] Require Google sign-in for external collaborators
* [ ] Limit who can move content from shared drives
* [ ] Control content sharing in new shared drives
* [ ] Disable access to offline docs
* [ ] Disable desktop access to Drive
* [ ] Don't allow Google Docs add-ons
* [ ] Block or warn on sharing files with sensitive data
* [ ] Ensure DLP policies are configured

### Gmail

* [ ] Authenticate email with SPF, DKIM, and DMARC
* [ ] Set up inbound email gateways to work with SPF
* [ ] Enforce TLS with your partner domains
* [ ] Require sender authentication for all approved senders
* [ ] Configure MX records for correct mail flow
* [ ] Disable IMAP/POP access
* [ ] Disable automatic forwarding
* [ ] Enable comprehensive mail storage
* [ ] Don't bypass spam filters for internal senders
* [ ] Add spam headers setting to all default routing rules
* [ ] Enable enhanced pre-delivery message scanning
* [ ] Enable external recipients warnings
* [ ] Enable additional attachment protection
* [ ] Enable additional link and external content protection
* [ ] Monitor and tune compliance rules to help prevent spam and phishing
* [ ] Scan and block emails with sensitive data

### Google Groups

* [ ] Use groups designed for security
* [ ] Add security conditions to admin roles
* [ ] Set up private access to your groups
* [ ] Limit group creation to admins
* [ ] Customize your group access settings
* [ ] Enable spam moderation for your groups

### Sites

* [ ] Block sharing sites outside the domain

### Vault

* [ ] Treat accounts with Vault privileges as sensitive
* [ ] Regularly audit Vault activity


## Additional Considerations

* [ ] Consider using [Advanced Gmail security](https://support.google.com/a/topic/2683828)
* [ ] Regularly visit the Security Center to review your security posture, investigate incidents and take action based on that information.
* [ ] Regularly monitor the activity and security logs provided in the Admin portal.

## Validation

* [ ] Validate that only the right people have the right access to data
* [ ] Validate that external sharing configuration is set up
* [ ] Validate that third-party apps access is restricted
* [ ] Validate that email security settings are in place and activity is being monitored

## References

1. [Directive on Security Management - Appendix B: Mandatory Procedures for Information Technology Security Control](https://www.tbs-sct.gc.ca/pol/doc-eng.aspx?id=32611&section=procedure&p=B), subsections B.2.3.3, B.2.3.7
2. [SPIN 2017-01](https://www.canada.ca/en/treasury-board-secretariat/services/access-information-privacy/security-identity-management/direction-secure-use-commercial-cloud-services-spin.html), subsection 6.2.3
3. CSE Top 10 #3
4. Refer to [CCCS ITSP.30.031 V2 User Authentication Guidance for Information Technology Systems](https://cyber.gc.ca/en/guidance/user-authentication-guidance-information-technology-systems-itsp30031-v3)
5. Refer to the [Guidance on Cloud Authentication for the Government of Canada](https://intranet.canada.ca/wg-tg/cagc-angc-eng.asp)
6. Refer to the [Recommendations for Two-Factor User Authentication Within the Government of Canada Enterprise Domain](https://intranet.canada.ca/wg-tg/rtua-rafu-eng.asp)
7. Related security controls: AC‑2, AC‑2(1), AC‑3, AC‑5, AC‑6, AC‑6(5), AC‑6(10), AC‑7, AC‑9, AC‑19, AC‑20(3), IA‑2, IA‑2(1), IA‑2(2), IA‑2(11), IA‑4, IA‑5, IA‑5(1), IA‑5(6), IA‑5(7), IA‑5(13), IA‑6, IA‑8
   * AU-2, CM-1, CM-2, CM-6, CM-7, CM-8, CM-10, CM-11, SC-7, SC-7(3), SC-7(4), SC-18, SC-20, SC-21, SI-3, SI-8
