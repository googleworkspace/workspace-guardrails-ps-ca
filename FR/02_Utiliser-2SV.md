# Utiliser l’authentification en deux étapes
([Retourner](/README.md#mesures-de-sécurité-dinformatique-en-nuage-du-gc-pour-google-workspace) | [English](/EN/02_Use_2Step_Verification.md))

## Objectif

La vérification en deux étapes place une barrière supplémentaire entre votre entreprise et les cybercriminels qui tentent de voler des noms d'utilisateur et des mots de passe pour accéder aux données de l'entreprise. L'activation de la vérification en deux étapes est la mesure la plus importante que vous puissiez prendre pour protéger votre entreprise.

Avec la vérification en deux étapes, vos utilisateurs se connectent à leur compte en deux étapes avec quelque chose qu'ils connaissent (leur mot de passe) et quelque chose qu'ils possèdent (leur téléphone ou une clé de sécurité).

Lorsque vous configurez la vérification en deux étapes, vous choisissez le deuxième facteur de vérification pour vos utilisateurs:
* [ ] Clés de sécurité
* [ ] Invite Google
* [ ] Google Authenticator et autres générateurs de codes de vérification
* [ ] Codes de secours
* [ ] SMS ou appel téléphonique

## Principales considérations

* [ ] Appliquer la vérification en deux étapes pour les [administrateurs et les utilisateurs clés](https://support.google.com/a/answer/175197?hl=fr&ref_topic=2759193).
* [ ] Envisager d'utiliser des clés de sécurité ou des alternatives telles que l'invite Google ou l'authentificateur Google. Les [Recommandations pour l'authentification des utilisateurs à deux facteurs dans le domaine d'entreprise du gouvernement du Canada](https://intranet.canada.ca/wg-tg/rtua-rafu-fra.asp) recommandent, au minimum, de combiner :
  * un nom d'utilisateur et un mot de passe de niveau 2 avec un téléphone intelligent géré par le GC à l'aide d'une notification push ou d'une application de mot de passe à usage unique (OTP);
  * un nom d’utilisateur et un mot de passe de niveau 2 avec un appareil OTP.

Si vous utilisez un fournisseur d'identité tiers:

* [ ] Si vous utilisez un fournisseur d'identité tiers pour authentifier les utilisateurs pour accéder aux produits Google et l'authentification unique (SSO) est activée pour votre organisation de niveau supérieur, par défaut, la vérification en deux étapes de Google ne s'applique pas lorsque les utilisateurs se connectent via ce service SSO. Remarque: vous pouvez définir une stratégie pour autoriser des défis d'authentification supplémentaires basés sur les risques et la vérification en deux étapes (2SV) (si configurée).
* [ ] Les super-administrateurs n'utilisent pas l'authentification unique lorsqu'ils se connectent à leurs comptes d'administrateur. S'ils sont inscrits à 2SV, ils doivent fournir un deuxième facteur d'authentification lorsqu'ils se connectent.

## Validation

* [ ] Confirmer que la vérification en deux étapes est activée sur les comptes.

## Références

1. [Directive sur la gestion de la sécurité, annexe B : Procédures obligatoires relatives aux mesures de sécurité de la technologie de l’information](https://www.tbs-sct.canada.ca/pol/doc-fra.aspx?id=32611), sous-section B.2.3.2.4.
3. [AMOPS 2017-01](https://www.canada.ca/en/treasury-board-secretariat/services/access-information-privacy/security-identity-management/direction-secure-use-commercial-cloud-services-spin.html), section 6.2.3
4. Les 10 principales mesures de sécurité du CST, numéro 3.
5. Voir le [Guide sur l’authentification des utilisateurs dans les systèmes de technologie de l’information (ITSP.30.031 v3)](https://cyber.gc.ca/fr/orientation/guide-sur-lauthentification-des-utilisateurs-dans-les-systemes-de-technologie-de)
6. [Voir Sécurisez vos comptes et vos appareils avec une authentification multifacteur (ITSAP.30.030)](https://cyber.gc.ca/fr/orientation/securisez-vos-comptes-et-vos-appareils-avec-une-authentification-multifacteur).
7. Voir [l’Orientation sur l’authentification du nuage à l’intention du gouvernement du Canada](https://intranet.canada.ca/wg-tg/cagc-angc-fra.asp)
8. Voir les [Recommandations pour l’authentification de l’utilisateur à deux facteurs au sein du domaine opérationnel du gouvernement du Canada](https://intranet.canada.ca/wg-tg/rtua-rafu-fra.asp)
9. Mesures de sécurité connexes : AC-2, AC-2(1), AC-3, AC-5, AC-6, AC-6(5), AC-6(10), AC-7, AC-9, AC-19, AC-20(3), IA-2, IA-2(1), IA-2(2), IA-2(11), IA-4, IA-5, IA-5(1), IA-5(6), IA-5(7), IA-5(13), IA-6, IA-8.
   * AU-2, CM-1, CM-2, CM-6, CM-7, SC-20, SC-21

