# Activer la journalisation et la surveillance
([Retourner](/README.md#mesures-de-sécurité-dinformatique-en-nuage-du-gc-pour-google-workspace) | [English](/EN/04_Enable-Logging-and-Monitoring.md))

## Objectif

Surveiller en permanence les événements et les performances du système et inclure une fonction de journal d'audit de sécurité dans tous les systèmes d'information pour permettre la détection des incidents. Il est essentiel qu'un niveau adéquat de journalisation et de reporting soit en place, y compris une fonction de journal d'audit de sécurité dans tous les systèmes d'information hébergés dans l'environnement cloud et pour les charges de travail basées sur le cloud.

## Principales considérations

### Journalisation

* [ ] Assurer que seuls les administrateurs ont accès à [l'outil d'investigation de sécurité](https://support.google.com/a/answer/7575955?hl=fr).
* [ ] Tirer profit du journal d'audit de l'administrateur pour consulter l'historique de chaque tâche effectuée dans la console d'administration Google: quel administrateur a effectué la tâche, la date et l'adresse IP à partir de laquelle l'administrateur s'est connecté.
* [ ] Assurer de [créer et de gérer des règles d'activité](https://support.google.com/a/answer/9275024?hl=fr) pour aider à prévenir, détecter et résoudre les problèmes de sécurité plus rapidement et plus efficacement.
* [ ] Assurer de [créer et de gérer des règles de création de rapports](https://support.google.com/a/answer/9908423?hl=fr) pour configurer des alertes basées sur les données d'événement de journal.
* [ ] Identifier les événements au sein de la solution qui doivent être audités conformément à la [journalisation des événements du GC](https://www.gcpedia.gc.ca/gcwiki/images/e/e3/GC_Event_Logging_Strategy.pdf).

### Surveillance

Le Centre de sécurité fournit des informations et des analyses de sécurité avancées, ainsi qu'une visibilité et un contrôle accrus sur les problèmes de sécurité affectant votre domaine.

* [ ] Visiter régulièrement le [Centre de sécurité](https://support.google.com/a/answer/7492003?hl=fr) pour examiner votre posture de sécurité, enquêter sur les incidents et prendre des mesures en fonction de ces informations.
* [ ] Surveiller en permanence les événements et les performances du système. Assurer que les rapports sont examinés au moins une fois par semaine, y compris :
  * [Rapports d'utilisateurs : comptes](https://support.google.com/a/answer/4580176?hl=fr)
  * [Rapports d'utilisateurs : utilisation de l'application](https://support.google.com/a/answer/4579578?hl=fr&ref_topic=9026833)
  * [Rapports d'utilisateurs : sécurité](https://support.google.com/a/answer/6000269?hl=fr&ref_topic=9026833)
  * [Rapport d'incidents DLP](https://support.google.com/a/answer/9304818?hl=fr&ref_topic=7492004)

* [ ] Tirer profit du [tableau de bord de sécurité](https://support.google.com/a/answer/7492534?hl=fr&ref_topic=7492004) pour afficher un aperçu des données de plusieurs rapports du centre de sécurité.
* [ ] Tirer profit de [l'outil d'investigation de sécurité](https://support.google.com/a/answer/7575955?hl=fr) pour identifier, trier et prendre des mesures concernant les problèmes de sécurité et de confidentialité de votre domaine. Par exemple, vous pouvez utiliser l'outil d'investigation pour:
  * Accéder aux données sur les appareils.
  * Accéder aux données du journal des appareils pour obtenir une vue claire des appareils et des applications utilisés pour accéder à vos données.
  * Accéder aux données sur les messages Gmail, y compris le contenu des e-mails.
  * Accéder aux données du journal Gmail pour rechercher et effacer les e-mails malveillants, marquer les e-mails comme spam ou hameçonnage, ou envoyer des e-mails aux boîtes de réception des utilisateurs.
  * Afficher les résultats de recherche qui répertorient les utilisateurs suspendus.
  * Accéder aux données du journal Drive pour enquêter sur le partage de fichiers dans votre organisation, enquêter sur la création et la suppression de documents, rechercher qui a accédé aux documents, et plus encore.
* [ ] Tirer profit de la page [État de la sécurité](https://support.google.com/a/answer/7492705?hl=fr) pour obtenir une meilleure visibilité sur votre console d'administration et mieux comprendre et gérer les risques de sécurité.
* [ ] Configurer les alertes et les notifications à envoyer au contact/à l'équipe appropriée dans l'organisation.
* [ ] Configurer ou utiliser une source de temps faisant autorité pour l'horodatage des enregistrements d'audit générés par les composants de votre solution.
* [ ] Élaborer un plan pour réagir et comprendre l'impact des incidents de sécurité, conformément au [Plan de gestion des événements de cybersécurité du GC](https://www.canada.ca/fr/secretariat-conseil-tresor/services/acces-information-protection-reseignements-personnels/gestion-securite-identite/plan-gestion-evenements-cybersecurite-gouvernement-canada.html).
* [ ] Établir un protocole d'entente pour les services défensifs et les services de protection contre les menaces avec CCCS.

## Considérations supplémentaires

* [ ] Envisager l'utilisation d'une solution de journalisation centrale chaque fois que possible. Les fonctionnalités qui automatisent l'analyse des événements et des comportements et offrent des alertes en temps réel peuvent aider à identifier les menaces et les incidents de sécurité potentiels.
* [ ] Envisager [l'exportation des journaux](https://support.google.com/a/answer/9320190?hl=fr) et des rapports d'utilisation dans Google Workspace vers les services Google Cloud Platform.
* [ ] Effectuer un audit administratif pour le centre de sécurité. De nombreuses tâches du centre de sécurité sont enregistrées via la source de données des événements du journal d'administration dans l'outil d'investigation de sécurité. Ces données de journal vous permettent de suivre l'historique des tâches effectuées dans votre console d'administration Google, y compris quel administrateur a effectué les tâches.

## Validation

* [ ] Vérifier que la stratégie de journalisation des événements est implémentée.
* [ ] Vérifier que les journaux d'événements sont générés.
* [ ] Vérifier que les informations de contact de sécurité ont été configurées pour recevoir des alertes et des notifications.
* [ ] Valider qu'un plan est mis en place pour répondre aux incidents.

## Références

1. [Directive sur la gestion de la sécurité, annexe B : Procédures obligatoires relatives aux mesures de sécurité de la technologie de l’information](https://www.tbs-sct.canada.ca/pol/doc-fra.aspx?id=32611), sous-section B.2.3.2.8.
2. [AMOPS 2017-01](https://www.canada.ca/en/treasury-board-secretariat/services/access-information-privacy/security-identity-management/direction-secure-use-commercial-cloud-services-spin.html), sections 6.3 et 6.3.1.
3. Les 10 principales mesures de sécurité du CST, numéro 1, 5 et 8.
4. Voir l’[Orientation sur la journalisation des événements du GC](https://www.gcpedia.gc.ca/gcwiki/images/e/e3/GC_Event_Logging_Strategy.pdf)
5. Mesures de sécurité connexes : AU-2, AU-3, AU-6, AU-8, AU-9, AU-9(4), AU-12, SI-2, SI-4.


