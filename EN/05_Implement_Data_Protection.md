# Implement Data Protection
([Return](/README.md) | [Français](/FR/05_Mettre-en-œuvre-la-protection-des-données.md))

## Objective

Safeguard information and assets hosted in cloud, from unauthorized access, use, disclosure, modification, disposal, transmission, or destruction throughout their life cycle.

## Key Considerations

* [ ] Seek guidance from privacy and access to information officials within institutions before storing personal information in cloud-based environments.
* [ ] Verify location of service, in accordance with Section 4.4.1.10 of the [Directive on Service and Digital](https://www.tbs-sct.gc.ca/pol/doc-eng.aspx?id=32601)
* [ ] Ensure data in transit is encrypted by default (e.g. TLS v1.2, etc.).
* [ ] Leverage encryption mechanisms to protect the confidentiality and integrity of data hosted in the cloud service.
* [ ] Use CSE-approved cryptographic algorithms and protocols, in accordance with [40.111](https://cyber.gc.ca/en/guidance/cryptographic-algorithms-unclassified-protected-and-protected-b-information-itsp40111) and [40.062](https://www.cse-cst.gc.ca/en/system/files/pdf_documents/itsp.40.062-eng.pdf).
* [ ] Enable Google Workspace DLP policies for Gmail, Drive and Chat content to be scanned for specific types of data, such as Social Insurance Numbers, credit card numbers, passwords and security markings.
* [ ] Apply classification labels to Drive files based on detection of sensitive context using DLP rules.
* [ ] Follow data protection considerations for each service as decribed in [Perfom Service Hardening](/EN/06_Perform_Service_Hardening.md).
* [ ] For mobile devices, review the list of recommendations in the [Device management security checklist](https://support.google.com/a/answer/7422256).
* [ ] Use [Vault](https://support.google.com/a/answer/2462365?hl=en) to perform information governance and eDiscovery tasks.

## Additional Considerations

* [ ] Consider using [Client-Side Encryption](https://support.google.com/a/answer/10741897?hl=en) to use your own encryption keys to encrypt your organization's data.
* [ ] Consider deploying [BeyondCorp Enterprise](https://support.google.com/a/answer/10104463) for threat and data protection for Chrome users.
* [ ] Consider implementing [Advanced Gmail security](https://support.google.com/a/topic/2683828?hl=en&ref_topic=2683865).
* [ ] Consider enabling [data insights report](https://support.google.com/a/answer/10324934?hl=en&ref_topic=9646660) to receive data protection rule recommendations.
* [ ] Consider [appliying automated classification with DLP rules](https://support.google.com/a/answer/9843931?hl=en&ref_topic=9646660).
* [ ] Control document sharing by domains with allow list or deny list.
* [ ] Treat accounts with Vault privileges as sensitive and regularly audit Vault activity.
* [ ] Ensure directory data access is externally restricted.

## Validation

* [ ] Confirm protected data is being blocked or alerted as intended.
* [ ] Confirm labels are being applied correctly based on protected data.
* [ ] Confirm Vault retention policies are in place where appropriate.
* [ ] Validate that sensitive data is being identified and protected.

## References

1. [Directive on Security Management - Appendix B: Mandatory Procedures for Information Technology Security Control](https://www.tbs-sct.gc.ca/pol/doc-eng.aspx?id=32611&section=procedure&p=B), subsections B.2.3.4
2. [SPIN 2017-01](https://www.canada.ca/en/treasury-board-secretariat/services/access-information-privacy/security-identity-management/direction-secure-use-commercial-cloud-services-spin.html), subsection 6.2.4
3. Refer to the cryptography guidance in [40.111](https://cyber.gc.ca/en/guidance/cryptographic-algorithms-unclassified-protected-and-protected-b-information-itsp40111) and [40.062](https://www.cse-cst.gc.ca/en/system/files/pdf_documents/itsp.40.062-eng.pdf).
4. Refer to the guidance in [Considerations for Cryptography in Commercial Cloud Services](https://www.canada.ca/en/government/system/digital-government/modern-emerging-technologies/cloud-services/government-canada-consideration-use-cryptography-in-cloud.html).
5. Refer to Section 4.4.1.10 of the [Directive on Service and Digital](https://www.tbs-sct.gc.ca/pol/doc-eng.aspx?id=32601)
6. Related security controls: SC‑8, SC‑8(1), SC‑12, SC‑13, SC‑17, SC‑28, SC‑28(1)
   * CA-7, AC-20, SA-9, CA-7, SI-4, MP-2, MP-7, AU-11
