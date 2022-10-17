# Exécuter le renforcement des appareils
([Retourner](/README.md#mesures-de-sécurité-dinformatique-en-nuage-du-gc-pour-google-workspace) | [English](/EN/07_Perform_Device_Hardening.md))

## Objectif

La posture de sécurité des appareils utilisés pour accéder un service doit être prise en compte. Au minimum, les entreprises doivent s'assurer que les appareils sont entièrement corrigés, n'utilisent pas de privilèges administratifs, ont mis en place des défenses contre les logiciels malveillants et collectent des journaux de sécurité.

En tant qu'administrateur, vous pouvez aider à protéger les données professionnelles sur les appareils personnels des utilisateurs (BYOD), et sur les appareils détenus par l'entreprise à l'aide des fonctionnalités et des paramètres de gestion des points de terminaison de Google. D'autres fonctionnalités de sécurité offrent une protection renforcée des comptes, un contrôle d'accès granulaire et une protection des données.

## Principales considérations

* [ ] Empêcher tout appareil non autorisé d'accéder à des informations professionnelles ou personnelles sensibles.
* [ ] Utiliser les points de terminaison gérés par GC et valider que l'appareil est conforme, par exemple en exigeant une version minimale et prise en charge du système d'exploitation.
* [ ] Conformément à l'[AMPTI 2018-03](https://www.canada.ca/fr/gouvernement/systeme/gouvernement-numerique/technologiques-modernes-nouveaux/avis-mise-oeuvre-politique/directive-migration-configuration-systeme-exploitation-bureau-windows10.html), lors de l'utilisation d'appareils Windows 10, la version et la configuration minimales de Windows 10 GC telles que spécifiées sur la page de configuration de base de [Windows 10 du GC](https://gcconnex.gc.ca/groups/profile/12903340/wtd-common-desktop-operating-environment-environnement-dexploitation-commun-des-ordinateurs-de-bureau-des-atmt?language=en#20998653) (accessible uniquement sur le réseau du gouvernement du Canada) doivent être mises en œuvre. La norme de configuration minimale du GC prescrit les normes de configuration de Windows 10 qui sont nécessaires pour maintenir la sécurité des réseaux du GC et des appareils technologiques en milieu de travail.
* [ ] Définir des règles pour automatiser les tâches de gestion des appareils et recevoir des alertes de sécurité.
* [ ] Assurer de suivre les consignes établies pour la [gestion des points de terminaison Google](https://support.google.com/a/topic/24642?hl=fr&ref_topic=10012113).

## Gestion des appareils mobiles

* [ ] Assurer que les politiques de gestion des appareils mobiles sont configurées pour exiger des configurations de sécurité avancées pour vous protéger contre les attaques Internet de base
* [ ] Assurer que les appareils mobiles nécessitent l'utilisation d'un mot de passe
* [ ] Assurer que la politique de mot de passe de l'appareil mobile est configurée, conformément aux directives sur les mots de passe du GC.
* [ ] Bloquer les appareils compromis
* [ ] Verrouiller ou effacer les données d'entreprise des appareils manquants
* [ ] Gérer les applications Android/iOS utilisées pour le travail
* [ ] Exiger le chiffrement de l'appareil
* [ ] Appliquer les restrictions d'appareil
* [ ] Bloquer automatiquement les appareils mobiles qui ne sont pas conformes à vos politiques
* [ ] Bloquer les applications mobiles potentiellement dangereuses

## Ordinateurs qui accèdent aux données professionnelles

* [ ] Activer la vérification des points de terminaison
* [ ] Restreindre Google Drive pour ordinateur aux appareils appartenant à l'entreprise
* [ ] Configurer le fournisseur d'informations d'identification Google pour Windows (GCPW) pour permettre aux utilisateurs de se connecter aux ordinateurs Windows 10 avec leur compte Google professionnel (le cas échéant)
* [ ] Restreindre les privilèges des utilisateurs sur les ordinateurs Windows appartenant à l'entreprise

## Plus de considérations de sécurité pour tous les appareils

* [ ] Empêcher l'accès non autorisé au compte d'un utilisateur
* [ ] Utiliser l'accès contextuel pour autoriser conditionnellement l'accès aux applications Google
* [ ] Identifier les données sensibles dans Google Drive, Docs, Sheets, Slides et Gmail

## Validation

* [ ] Valider que les restrictions d'appareil sont en place
* [ ] Valider que le cryptage de l'appareil est activé
* [ ] Valider que les applications iOS et Android sont gérées
* [ ] Valider que la vérification des points de terminaison est activée

## Références

1. [Directive sur la gestion de la sécurité, annexe B : Procédures obligatoires relatives aux mesures de sécurité de la technologie de l’information](https://www.tbs-sct.canada.ca/pol/doc-fra.aspx?id=32611).
2. [AMOPS 2017-01](https://www.canada.ca/fr/gouvernement/systeme/gouvernement-numerique/innovations-gouvernementales-numeriques/services-informatique-nuage/orientation-utilisation-securisee-services-commerciaux-informatique-nuage-amops.html).

