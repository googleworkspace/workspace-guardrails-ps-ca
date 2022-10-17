# Mettre en œuvre la protection des données
([Retourner](/README.md#mesures-de-sécurité-dinformatique-en-nuage-du-gc-pour-google-workspace) | [English](/EN/05_Implement_Data_Protection.md))

## Objectif

Protéger les informations et les actifs hébergés dans le cloud contre tout accès, utilisation, divulgation, modification, élimination, transmission ou destruction non autorisés tout au long de leur cycle de vie.

## Principales considérations

* [ ] Demander des conseils aux responsables de la confidentialité et de l’accès à l’information dans les institutions avant de stocker des informations personnelles dans des environnements d’informatique en nuage.
* [ ] Vérifier l'emplacement du service, conformément à la section 4.4.1.10 de la [Directive sur les services et le numérique](https://www.tbs-sct.canada.ca/pol/doc-fra.aspx?id=32601).
* [ ] Veiller que les données en transit sont chiffrées par défaut (par exemple, TLS v1.2, etc.).
* [ ] Appliquer des mécanismes de chiffrement pour protéger la confidentialité et l'intégrité des données hébergées dans le service d’informatique en nuage.
* [ ] Utiliser des algorithmes et des protocoles cryptographiques approuvés par le CST, conformément aux [40.111](https://cyber.gc.ca/fr/orientation/algorithmes-cryptographiques-pour-linformation-non-classifie-protege-et-protege-b) et [40.062](https://www.cse-cst.gc.ca/fr/system/files/pdf_documents/itsp.40.062-fra.pdf).
* [ ] Activer les politiques de la prévention de la perte de données (PPD) Google Workspace pour que le contenu Gmail, Drive et Chat soit analysé pour des types de données spécifiques, tels que les numéros d'assurance sociale, les numéros de carte de crédit, les mots de passe et les marques de sécurité.
* [ ] Appliquer des étiquettes de classification aux fichiers Drive en fonction de la détection du contexte sensible à l'aide des règles PPD.
* [ ] Suivre les considérations de protection des données pour chaque service, comme décrit dans [Exécuter le renforcement des services](06_Exécuter-le-renforcement-des-services.md).
* [ ] Pour les appareils mobiles, consultez la liste des recommandations dans la [liste de vérification de la sécurité de la gestion des appareils](https://support.google.com/a/answer/7422256?hl=fr).
* [ ] Utiliser [Vault](https://support.google.com/a/answer/2462365?hl=fr) pour effectuer des tâches de gouvernance des informations et d'eDiscovery.

## Considérations supplémentaires

* [ ] Envisagez d'utiliser le [chiffrement côté client](https://support.google.com/a/answer/10741897?hl=fr) pour utiliser vos propres clés de chiffrement afin de chiffrer les données de votre organisation.
* [ ] Envisager de mettre en œuvre la [sécurité avancée](https://support.google.com/a/topic/2683828?hl=fr&ref_topic=2683865) de gmail .
* [ ] Envisager d'activer le [rapport d'informations sur les données](https://support.google.com/a/answer/10324934?hl=fr&ref_topic=9646660) pour recevoir des recommandations sur les règles de protection des données.
* [ ] Envisager d'appliquer une [classification automatisée avec des règles PPD/DLP](https://support.google.com/a/answer/9843931?hl=fr&ref_topic=9646660).
* [ ] Contrôler le partage de documents par domaines avec une liste d'autorisation ou une liste de refus.
* [ ] Traiter les comptes avec des privilèges Vault comme sensibles et auditez régulièrement l'activité Vault.
* [ ] Assurer que l'accès aux données du répertoire est restreint de l'extérieur.

## Validation

* [ ] Confirmer que les données protégées sont bloquées ou alertent comme prévu.
* [ ] Confirmer que les étiquettes sont appliquées correctement en fonction des données protégées.
* [ ] Confirmer que des politiques de conservation Vault sont en place, le cas échéant.
* [ ] Valider que les données sensibles sont identifiées et protégées.

## Références

1. [Directive sur la gestion de la sécurité, annexe B : Procédures obligatoires relatives aux mesures de sécurité de la technologie de l’information](https://www.tbs-sct.canada.ca/pol/doc-fra.aspx?id=32611), sous-section B.2.3.4.
2. [AMOPS 2017-01](https://www.canada.ca/en/treasury-board-secretariat/services/access-information-privacy/security-identity-management/direction-secure-use-commercial-cloud-services-spin.html), section 6.2.4.
3. Voir les conseils en matière de cryptographie sous les publications [40.111](https://cyber.gc.ca/fr/orientation/algorithmes-cryptographiques-pour-linformation-non-classifie-protege-et-protege-b) et [40.062](https://www.cse-cst.gc.ca/en/system/files/pdf_documents/itsp.40.062-eng.pdf).
4. Voir les conseils dans [Considérations relatives à l’utilisation de la cryptographie dans les services d’informatique en nuage commerciaux](https://www.canada.ca/fr/gouvernement/systeme/gouvernement-numerique/technologiques-modernes-nouveaux/services-informatique-nuage/consideration-utilisation-de-la-crrptographie-dans-les-services-informatique-en-nauge.html)
5. Voir la section 4.4.1.10 de la [Directive sur les services et le numérique](https://www.tbs-sct.gc.ca/pol/doc-fra.aspx?id=32601)
6. Mesures de sécurité connexes : SC 8, SC 8(1), SC 12, SC 13, SC 17, SC 28, SC 28(1).
   * CA-7, AC-20, SA-9, CA-7, SI-4, MP-2, MP-7, AU-11
