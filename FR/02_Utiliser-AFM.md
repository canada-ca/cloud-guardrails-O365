# Utiliser l’authentification à facteurs multiples

([Retourner](README.md#mesures-de-sécurité-initiales))

## Objectif

L’authentification à facteurs multiples (AFM) est une méthode d’authentification qui requiert l’utilisation de plus d’une méthode de vérification, comme :

* quelque chose que vous connaissez (habituellement un mot de passe);
* quelque chose que vous avez (un appareil de confiance comme un téléphone mobile);
* quelque chose que vous êtes (données biométriques).

L’AFM ajoute une deuxième couche de sécurité à l’ouverture de session et aux opérations des utilisateurs. Elle offre une couche supplémentaire de protection à une stratégie de mot de passe robuste en fournissant un moyen de « contre-vérifier » que vous êtes réellement la personne que vous affirmez être lorsque vous utilisez des services en ligne. Avec l’AFM en place, les comptes d’utilisateur Office 365 sont protégés contre l’accès non autorisé, même si le mot de passe d’un utilisateur est compromis.

## Principales considérations

* [Mettre en œuvre](https://docs.microsoft.com/fr-ca/microsoft-365/admin/security-and-compliance/secure-your-business-data?view=o365-worldwide) un mécanisme d’authentification à facteurs multiples pour les interfaces externes et l’accès au réseau à distance (nuage) conformément aux stratégies d’accès conditionnel. Les [Recommandations pour l’authentification de l’utilisateur à deux facteurs au sein du domaine opérationnel du gouvernement du Canada](https://intranet.canada.ca/wg-tg/rtua-rafu-fra.asp), lesquelles recommandent, à tout le moins, d’utiliser l’une des combinaisons suivantes :
  * un ID utilisateur et un mot de passe de niveau 2 avec un téléphone intelligent géré par le GC au moyen d’une notification poussée ou d’une application de mot de passe à usage unique;
  * un ID utilisateur et un mot de passe de niveau 2 avec un appareil protégé par un mot de passe à usage unique.
* Veiller à ce que l’authentification à facteurs multiples soit activée pour tous les utilisateurs occupant des rôles d’administrateur.

## Validation

* Confirmer que l’authentification à facteurs multiples est activée pour les comptes.

## Références

1. Directive sur la gestion de la sécurité, annexe B : Procédures obligatoires relatives aux mesures de sécurité de la technologie de l’information sous-section B.2.3.2.4.
2. [AMOPS 2017-01](https://www.canada.ca/en/treasury-board-secretariat/services/access-information-privacy/security-identity-management/direction-secure-use-commercial-cloud-services-spin.html), section 6.2.3
3. Les 10 principales mesures de sécurité du CST, numéro 3.
4. Voir le [Guide sur l’authentification des utilisateurs dans les systèmes de technologie de l’information (ITSP.30.031 v3)](https://cyber.gc.ca/fr/orientation/guide-sur-lauthentification-des-utilisateurs-dans-les-systemes-de-technologie-de)
5. [Voir Sécurisez vos comptes et vos appareils avec une authentification multifacteur (ITSAP.30.030)](https://cyber.gc.ca/fr/orientation/securisez-vos-comptes-et-vos-appareils-avec-une-authentification-multifacteur).
6. Voir [l’Orientation sur l’authentification du nuage à l’intention du gouvernement du Canada](https://intranet.canada.ca/wg-tg/cagc-angc-fra.asp)
7. Voir les [Recommandations pour l’authentification de l’utilisateur à deux facteurs au sein du domaine opérationnel du gouvernement du Canada](https://intranet.canada.ca/wg-tg/rtua-rafu-fra.asp)
8. Mesures de sécurité connexes : AC-2, AC-2(1), AC-3, AC-5, AC-6, AC-6(5), AC-6(10), AC-7, AC-9, AC-19, AC-20(3), IA-2, IA-2(1), IA-2(2), IA-2(11), IA-4, IA-5, IA-5(1), IA-5(6), IA-5(7), IA-5(13), IA-6, IA-8.
