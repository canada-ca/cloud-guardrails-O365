# Utiliser l’authentification à facteurs multiples

## Objectif

L’authentification à facteurs multiples (AFM) est une méthode d’authentification qui requiert l’utilisation de plus d’une méthode de vérification, comme :
* quelque chose que vous connaissez (habituellement un mot de passe);
* quelque chose que vous avez (un appareil de confiance comme un téléphone mobile);
* quelque chose que vous êtes (données biométriques).

L’AFM ajoute une deuxième couche de sécurité à l’ouverture de session et aux opérations des utilisateurs. Elle offre une couche supplémentaire de protection à une stratégie de mot de passe robuste en fournissant un moyen de « contre-vérifier » que vous êtes réellement la personne que vous affirmez être lorsque vous utilisez des services en ligne. Avec l’AFM en place, les comptes d’utilisateur Office 365 sont protégés contre l’accès non autorisé, même si le mot de passe d’un utilisateur est compromis.

## Principales considérations

* [ ] [Mettre en œuvre]https://docs.microsoft.com/en-us/microsoft-365/admin/security-and-compliance/secure-your-business-data?view=o365-worldwide#setup) un mécanisme d’authentification à facteurs multiples pour les interfaces externes et l’accès au réseau à distance (nuage) conformément aux [Recommandations pour l’authentification de l’utilisateur à deux facteurs au sein du domaine opérationnel du gouvernement du Canada](https://intranet.canada.ca/wg-tg/rtua-rafu-eng.asp) lesquelles recommandent, à tout le moins, d’utiliser l’une des combinaisons suivantes :
* un ID utilisateur et un mot de passe de niveau 2 avec un téléphone intelligent géré par le GC au moyen d’une notification poussée ou d’une application de mot de passe à usage unique;
* un ID utilisateur et un mot de passe de niveau 2 avec un appareil protégé par un mot de passe à usage unique.

* [ ] Veiller à ce que l’authentification à facteurs multiples soit activée pour tous les utilisateurs occupant des rôles d’administrateur.

## Validation

* [ ] Confirmer que l’authentification à facteurs multiples est activée pour les comptes.

## Références

1. [SPIN 2017-01](https://www.canada.ca/en/treasury-board-secretariat/services/access-information-privacy/security-identity-management/direction-secure-use-commercial-cloud-services-spin.html), subsection 6.2.3
2. CSE Top 10 #3
3. Refer to [CCCS ITSP.30.031 V2 User Authentication Guidance for Information Technology Systems](https://cyber.gc.ca/en/guidance/user-authentication-guidance-information-technology-systems-itsp30031-v3)
4. Refer to the [Guidance on Cloud Authentication for the Government of Canada](https://intranet.canada.ca/wg-tg/cagc-angc-eng.asp)
5. Refer to the [Recommendations for Two-Factor User Authentication Within the Government of Canada Enterprise Domain](https://intranet.canada.ca/wg-tg/rtua-rafu-eng.asp)
6. Related security controls: AC‑2, AC‑2(1), AC‑3, AC‑5, AC‑6, AC‑6(5), AC‑6(10), AC‑7, AC‑9, AC‑19, AC‑20(3), IA‑2, IA‑2(1), IA‑2(2), IA‑2(11), IA‑4, IA‑5, IA‑5(1), IA‑5(6), IA‑5(7), IA‑5(13), IA‑6, IA‑8
