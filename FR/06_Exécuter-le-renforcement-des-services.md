# Exécuter le renforcement des services
([Retourner](/README.md#mesures-de-sécurité-dinformatique-en-nuage-du-gc-pour-google-workspace) | [English](/EN/06_Perform_Service_Hardening.md))

## Objectif

Réduire au minimum les services disponibles et contrôler la connectivité en désactivant les services et en supprimant les comptes inutiles des systèmes. Configurer Google Workspace et les appareils qui y ont accès pour renforcer la sécurité et la confidentialité des données de l'entreprise.

Des conseils de mise en œuvre sont fournis dans la [liste de contrôle de sécurité](https://support.google.com/a/answer/7587183?hl=fr).

## Principales considérations

### Applications
* [ ] Examiner l'accès des applications tierces aux services principaux
* [ ] Bloquer l'accès aux applications moins sécurisées
* [ ] Créer une liste d'applications de confiance
* [ ] Contrôler l'accès aux services principaux de Google

### Calendrier
* [ ] Limiter le partage de calendrier externe
* [ ] Avertir les utilisateurs lorsqu'ils invitent des invités externes

### Google Chat
* [ ] Limiter qui peut discuter en externe
* [ ] Avertir les utilisateurs lorsqu'ils discutent en dehors de leur domaine
* [ ] Définir une politique d'invitation au chat
* [ ] Définir et mettre en œuvre des règles prévention de la perte de données (DDP/DLP) pour protéger les données sensibles dans les messages et les fichiers dans Google Chat

### Navigateur Chrome ou Appareils Chrome OS
* [ ] Maintenir le navigateur Chrome ou Chrome OS à jour
* [ ] Définir les règles de base de l'appareil Chrome OS et du navigateur Chrome
* [ ] Définir les règles avancées du navigateur Chrome
* [ ] Définir une stratégie de navigateur Windows

### Drive
* [ ] Définir les options de partage pour votre domaine
* [ ] Définir la valeur par défaut pour le partage de lien
* [ ] Avertir les utilisateurs lorsqu'ils partagent un fichier en dehors de votre domaine
* [ ] Limiter l'accès aux fichiers aux destinataires uniquement
* [ ] Empêcher les utilisateurs de publier sur le Web
* [ ] Exiger la connexion à Google pour les collaborateurs externes
* [ ] Limiter les personnes autorisées à déplacer du contenu des lecteurs de partage
* [ ] Contrôler le partage de contenu dans les nouveaux lecteurs de partagés
* [ ] Désactiver l'accès aux documents hors connexion
* [ ] Désactiver l'accès du bureau à Drive
* [ ] Ne pas autoriser les modules complémentaires Google Docs
* [ ] Bloquer ou avertir du partage de fichiers contenant des données sensibles
* [ ] Assurer que les politiques DLP sont configurées

### Gmail
* [ ] Authentifier les courriels avec SPF, DKIM et DMARC
* [ ] Configurer des passerelles de messagerie entrantes pour fonctionner avec SPF
* [ ] Appliquez TLS avec vos domaines partenaires
* [ ] Exiger l'authentification de l'expéditeur pour tous les expéditeurs approuvés
* [ ] Configurer les enregistrements MX pour un flux de messagerie correct
* [ ] Désactiver l'accès IMAP/POP
* [ ] Désactiver le transfert automatique
* [ ] Activer le stockage complet du courrier
* [ ] Ne contournez pas les filtres anti-spam pour les expéditeurs internes
* [ ] Ajouter le paramètre d'en-têtes de spam à toutes les règles de routage par défaut
* [ ] Activer l'analyse améliorée des messages avant distribution
* [ ] Activer les avertissements des destinataires externes
* [ ] Activer la protection supplémentaire des pièces jointes
* [ ] Activer la protection supplémentaire des liens et du contenu externe
* [ ] Surveiller et ajuster les règles de conformité pour aider à prévenir le spam et le phishing
* [ ] Analyser et bloquer les courriels contenant des données sensibles

### Groupes Google

* [ ] Utiliser des groupes conçus pour la sécurité
* [ ] Ajouter des conditions de sécurité aux rôles d'administrateur
* [ ] Configurer un accès privé à vos groupes
* [ ] Limiter la création de groupes aux administrateurs
* [ ] Personnaliser les paramètres d'accès de votre groupe
* [ ] Activer la modération des spams pour vos groupes

### Sites

* [ ] Bloquer le partage des sites en dehors du domaine

### Vault

* [ ] Traiter les comptes avec des privilèges Vault comme sensibles
* [ ] Auditer régulièrement l'activité de Vault

## Considérations supplémentaires

* [ ] Envisager d'utiliser la [sécurité avancée de Gmail](https://support.google.com/a/topic/2683828?hl=fr)
* [ ] Visiter régulièrement le centre de sécurité pour examiner votre posture de sécurité, enquêter sur les incidents et prendre des mesures en fonction de ces informations.
* [ ] Surveiller régulièrement les journaux d'activité et de sécurité fournis dans le portail d'administration.

## Validation

* [ ] Valider que seules les bonnes personnes ont le droit d'accéder aux données
* [ ] Valider que la configuration du partage externe est configurée
* [ ] Valider que l'accès aux applications tierces est restreint
* [ ] Valider que les paramètres de sécurité des courriels sont en place et que l'activité est surveillée

## Références

1. [Directive sur la gestion de la sécurité, annexe B : Procédures obligatoires relatives aux mesures de sécurité de la technologie de l’information](https://www.tbs-sct.canada.ca/pol/doc-fra.aspx?id=32611), sous-sections B.2.3.3 et B.2.3.7.
2. [AMOPS 2017-01](https://www.canada.ca/en/treasury-board-secretariat/services/access-information-privacy/security-identity-management/direction-secure-use-commercial-cloud-services-spin.html), section 6.2.3.
3. Les 10 principales mesures de sécurité du CST, numéro 3.
4. Voir le [Guide sur l’authentification des utilisateurs dans les systèmes de technologie de l’information (ITSP.30.031 v3) du CCC](https://cyber.gc.ca/fr/orientation/guide-sur-lauthentification-des-utilisateurs-dans-les-systemes-de-technologie-de)
5. Voir l'[Orientation sur l’authentification du nuage à l’intention du gouvernement du Canada](https://intranet.canada.ca/wg-tg/cagc-angc-fra.asp)
6. Voir les [Recommandations pour l’authentification de l’utilisateur à deux facteurs au sein du domaine opérationnel du gouvernement du Canada](https://intranet.canada.ca/wg-tg/rtua-rafu-fra.asp)
7. Mesures de sécurité connexes : AC-2, AC-2(1), AC-3, AC-5, AC-6, AC-6(5), AC-6(10), AC-7, AC-9, AC-19, AC-20(3), IA-2, IA-2(1), IA-2(2), IA-2(11), IA-4, IA-5, IA-5(1), IA-5(6), IA-5(7), IA-5(13), IA-6, IA-8.
   * AU-2, CM-1, CM-2, CM-6, CM-7, CM-8, CM-10, CM-11, SC-7, SC-7(3), SC-7(4), SC-18, SC-20, SC-21, SI-3, SI-8
