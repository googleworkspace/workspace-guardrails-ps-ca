# Mettre en œuvre l'accès contextuel
([Retourner](/README.md#mesures-de-sécurité-dinformatique-en-nuage-du-gc-pour-google-workspace) | [English](/EN/03_Implement_Context_Aware_Access.md))

## Objectif

Grâce à l'accès contextuel, vous pouvez créer des politiques de contrôle d'accès granulaires aux applications en fonction d'attributs tels que l'identité de l'utilisateur, l'emplacement, l'état de sécurité de l'appareil et l'adresse IP.

[L'accès contextuel](https://support.google.com/a/answer/9275380?hl=fr) vous permet de contrôler les applications auxquelles un utilisateur peut accéder en fonction de son contexte, par exemple si son appareil est conforme à votre politique informatique.

## Principales considérations

* [ ] Assurer que les utilisateurs comprennent leurs responsabilités lorsqu'ils utilisent des appareils personnels pour accéder aux données et aux services, ainsi que les risques liés au partage de données professionnelles avec des utilisateurs non autorisés.
* [ ] Établir des [niveaux d'accès contextuels](https://support.google.com/a/answer/9262032?hl=fr&ref_topic=9262521) qui combinent des conditions et des valeurs qui définissent un contexte d'utilisateur ou d'appareil. Les niveaux d'accès définissent le contexte dans lequel les utilisateurs peuvent accéder aux applications en fonction de conditions telles que :
  * sous-réseau IP,
  * position géographique,
  * politique de l'appareil,
  * système d'exploitation de l'appareil ou
  * créer des spécifications de niveau d'accès personnalisées qui répondent à vos besoins spécifiques.
* [ ] Assurer que les niveaux d'accès contextuels établis répondent aux problèmes d'accès courants tels que:
  * bloquer ou exiger la vérification en deux étapes (2SV) pour toute tentative d'accès depuis l'extérieur du réseau de l'entreprise;
  * exiger la vérification en deux étapes pour les utilisateurs ayant des rôles administratifs;
  * exiger une vérification en deux étapes pour les tâches de gestion de l'espace de travail;
  * bloquer ou accorder l'accès à partir d'emplacements spécifiques;
  * bloquer les comportements de connexion à risque; et
  * nécessitant des appareils gérés par le GC pour des applications spécifiques en tenant compte de la catégorisation des données.
* [ ] Créer des niveaux d'accès à la console d'administration. Éviter un verrouillage et assurer qu'au moins un administrateur répond [aux critères d'accès](https://support.google.com/a/answer/10759654).
* [ ] Mettre en œuvre des politiques d'accès basées sur l'appareil et le statut de conformité pour autoriser ou bloquer l'accès aux applications et aux services.
* [ ] Utiliser l'outil d'investigation de sécurité pour surveiller et exécuter des recherches liées aux [événements du journal d'accès contextuel](https://support.google.com/a/answer/9394107?hl=fr&ref_topic=9262521) et prendre des mesures en fonction des résultats.

## Considérations supplémentaires

* [ ] Suivre les [bonnes pratiques pour déployer des stratégies d'accès contextuel](https://support.google.com/a/answer/9275380?hl=fr).
* [ ] Envisager d'appliquer [l'accès contextuel aux groupes](https://support.google.com/a/answer/9668676?hl=fr).
* [ ] Envisager d'appliquer des niveaux d'accès contextuels en [mode avancé](https://support.google.com/a/answer/11368990?hl=fr&ref_topic=9262521).
* [ ] Garantir l'accès au support en cas de lock-out. Si nécessaire, suivez les étapes pour [Permettre à des utilisateurs d'accéder à Customer Care Portal](https://support.google.com/a/answer/10759654?hl=fr).
* [ ] Pour l'accès basé sur l'appareil :
  * Envisager d'activer la [gestion avancée des appareils mobiles](https://support.google.com/a/answer/7396025?hl=fr&ref_topic=1734198) pour mieux contrôler l'accès aux données de votre organisation.
  * Envisager de mettre en œuvre des politiques de [prévention contre la perte de données](https://support.google.com/a/topic/7556687?hl=fr) pour protéger les données sensibles et contrôler les applications qui peuvent accéder aux données de Google Workspace.
  * Exiger une preuve d'identité supplémentaire lorsque les utilisateurs se connectent à leur compte Google avec la validation en deux étapes (2SV).
  * Suivre les bonnes pratiques de la liste de vérification de la [sécurité de la gestion des appareils](https://support.google.com/a/answer/7422256?hl=fr).
  * Envisager d'appliquer des niveaux d'accès basés sur la propriété ou le chiffrement de l'entreprise.
  * Envisager d'appliquer des niveaux d'accès en fonction de l'état de l'approbation ou du mot de passe.

## Validation
  * Vérifier que les niveaux d'accès contextuels sont en place et répondent aux exigences de sécurité.
  * Valider que les niveaux d'accès établis permettent de surveiller et de prévenir les connexions à risque.

## Références

1. [Directive sur la gestion de la sécurité, annexe B : Procédures obligatoires relatives aux mesures de sécurité de la technologie de l’information](https://www.tbs-sct.canada.ca/pol/doc-fra.aspx?id=32611), sous-sections B.2.3.1 et B.2.3.2.4.
2. [AMOPS 2017-01](https://www.canada.ca/en/treasury-board-secretariat/services/access-information-privacy/security-identity-management/direction-secure-use-commercial-cloud-services-spin.html), section 6.2.3.
3. Les 10 principales mesures de sécurité du CST, numéro 3.
4. Voir le [Guide sur l’authentification des utilisateurs dans les systèmes de technologie de l’information (ITSP.30.031 v3) du CCC](https://cyber.gc.ca/fr/orientation/guide-sur-lauthentification-des-utilisateurs-dans-les-systemes-de-technologie-de).
5. Voir l'[Orientation sur l’authentification du nuage à l’intention du gouvernement du Canada](https://intranet.canada.ca/wg-tg/cagc-angc-fra.asp).
6. Voir les [Recommandations pour l’authentification de l’utilisateur à deux facteurs au sein du domaine opérationnel du gouvernement du Canada](https://intranet.canada.ca/wg-tg/rtua-rafu-fra.asp).
7. Mesures de sécurité connexes : AC-2, AC-2(1), AC-3, AC-5, AC-6, AC-6(5), AC-6(10), AC-7, AC-9, AC-19, AC-20(3), IA-2, IA-2(1), IA-2(2), IA-2(11), IA-4, IA-5, IA-5(1), IA-5(6), IA-5(7), IA-5(13), IA-6, IA-8.
   * AU-2, CM-1, CM-2, CM-6, CM-7, SC-20, SC-21

