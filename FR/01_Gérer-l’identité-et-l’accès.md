# Gérer l'identité et l'accès
([Retourner](/README.md#mesures-de-sécurité-dinformatique-en-nuage-du-gc-pour-google-workspace) | [English](/EN/01_Manage-Identity-Access.md))

## Objectif

Gérer les identités et établir des politiques et des procédures de contrôle d'accès pour la gestion des privilèges administratifs.

## Principales considérations

### Identité

* [ ] Ajouter Cloud Identity à Google Workspace pour gérer les identités.
* [ ] Configurer les contrôles pour protéger les mots de passe conformément à la [Stratégie de mise en œuvre des lignes directrices sur les mots de passe du GC](https://www.gcpedia.gc.ca/gcwiki/images/c/c0/Implementation_Strategy_for_GC_Password_Guidance.pdf) (accessible uniquement sur le réseau du gouvernement du Canada).
* [ ] Configurer les comptes d'urgence (super administrateur) dans Google Workspace.
* [ ] Assurer qu'entre deux et quatre super administrateurs sont désignés.
* [ ] Activer l'alerte de mot de passe pour vous assurer que les utilisateurs n'utilisent pas leurs mots de passe d'entreprise sur d'autres sites.
* [ ] Suivre les bonnes pratiques de sécurité de Google [pour les comptes d'administrateur](https://support.google.com/a/answer/9011373).

Si vous utilisez un fournisseur d'identité tiers, tenez compte des bonnes pratiques suivantes pour votre configuration du Google Workspace :

* [ ] Maintenir des mots de passe forts pour les comptes du Google Workspace. Ces mots de passe sont moins susceptibles d'être utilisés, ils peuvent donc représenter une surface d'attaque.
* [ ] Activer l'authentification unique et assurer que votre fournisseur d'identité et tous les systèmes dont il dépend sont configurés en toute sécurité.
* [ ] Suivre les [bonnes pratiques de Google pour fédérer Google Cloud avec un fournisseur d'identité externe](https://cloud.google.com/architecture/identity/best-practices-for-federating).

### Accès

Implémenter un mécanisme pour identifier et authentifier de manière unique les utilisateurs organisationnels, les utilisateurs non organisationnels (le cas échéant) et les processus (par exemple, nom d'utilisateur et mot de passe).

* [ ] Exiger une vérification en deux étapes pour les utilisateurs.
* [ ] Assurer que les défis de connexion ont été configurés pour les tentatives de connexion suspectes.
* [ ] Appliquer des clés de sécurité, au moins pour les administrateurs et autres comptes de grande valeur, à l'aide d'une clé de sécurité ou d'un autre dispositif d'authentification physique.
* [ ] Appliquer la politique de mot de passe conformément aux directives du [GC sur les mots de passe](https://www.canada.ca/en/government/system/digital-government/password-guidance.html).
* [ ] Implémenter un accès basé sur les rôles et utiliser des rôles avec le moins de privilèges possible (par exemple, utilisez des rôles administratifs non globaux).
* [ ] Utiliser des comptes dédiés pour effectuer des tâches administratives.
* [ ] Contrôler qui peut accéder au portail d'administration, à Google Workspace et aux services Google.
* [ ] Interdire l'accès aux applications moins sécurisées.
* [ ] Bloquer l'accès aux comptes des particuliers.
* [ ] Examiner régulièrement les rapports et les alertes de sécurité, conformément à la mesure de sécurité [Activer la journalisation et la surveillance](04_Activer-la-journalisation-et-la-surveillance.md).
* [ ] Maintenir votre sécurité après le départ d'un collaborateur en suivant des [bonnes pratiques](https://support.google.com/a/answer/6329207?hl=fr&ref_topic=7558661).

## Considérations supplémentaires

* [ ] Exiger des collaborateurs externes qu'ils se connectent avec un compte Google. S'ils ne possèdent pas de compte Google, ils peuvent en créer un gratuitement.
* [ ] Envisager d'activer le programme [Protection Avancée](https://support.google.com/a/answer/9378686?hl=fr) pour protéger les comptes Google contre les attaques en ligne ciblées.
* [ ] Déterminer les restrictions d'accès et les exigences de configuration pour les dispositifs d'extrémité émis par le GC, y compris ceux des utilisateurs non privilégiés et privilégiés, et configurer les restrictions d'accès en conséquence.
* [ ] Assurer que le contrôle de session Google est configuré.

Si vous utilisez Azure Active Directory/O365:

* [ ] Empêcher l'utilisation des protocoles d'authentification hérités.
* [ ] Envisager d'activer la protection de l'identité (licence supplémentaire requise)
* [ ] Envisager de contrôler les tâches administratives avec la gestion des accès privilégiés (licence supplémentaire requise)
* [ ] Enquêter sur l'accès juste à temps pour permettre l'accès administratif au besoin (licence supplémentaire requise)

## Validation

* [ ] Confirmer qu'un plan et un processus de gestion des comptes privilégiés ont été documentés.
* [ ] Confirmer que la politique de mot de passe est conforme aux [directives sur les mots de passe du GC](https://www.canada.ca/en/government/system/digital-government/password-guidance.html) (accessible uniquement sur le réseau du gouvernement du Canada), le cas échéant.

## Références

1. [Directive sur la gestion de la sécurité, annexe B : Procédures obligatoires relatives aux mesures de sécurité de la technologie de l’information](https://www.tbs-sct.canada.ca/pol/doc-fra.aspx?id=32611) sous-sections B.2.3.1 et B.2.3.2.4.
2. [AMOPS 2017-01](https://www.canada.ca/en/treasury-board-secretariat/services/access-information-privacy/security-identity-management/direction-secure-use-commercial-cloud-services-spin.html), section 6.2.3
3. Les 10 principales mesures de sécurité du CST, numéro 3.
4. Voir le [Guide sur l’authentification des utilisateurs dans les systèmes de technologie de l’information (ITSP.30.031 v3)](https://cyber.gc.ca/fr/orientation/guide-sur-lauthentification-des-utilisateurs-dans-les-systemes-de-technologie-de)
5. Voir [l’Orientation sur l’authentification du nuage à l’intention du gouvernement du Canada](https://intranet.canada.ca/wg-tg/cagc-angc-fra.asp) (accessible seulement sur le réseau du gouvernement du Canada)
6. Voir les [Recommandations pour l’authentification de l’utilisateur à deux facteurs au sein du domaine opérationnel du gouvernement du Canada](https://intranet.canada.ca/wg-tg/rtua-rafu-fra.asp) (accessible seulement sur le réseau du gouvernement du Canada)
7. Mesures de sécurité connexes : AC-2, AC-2(1), AC-3, AC-5, AC-6, AC-6(5), AC-6(10), AC-7, AC-9, AC-19, AC-20(3), IA-2, IA-2(1), IA-2(2), IA-2(11), IA-4, IA-5, IA-5(1), IA-5(6), IA-5(7), IA-5(13), IA-6, IA-8.
   * AU-2, CM-1, CM-2, CM-6, CM-7, SC-20, SC-21
