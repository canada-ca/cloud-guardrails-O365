# Appliquer des politiques de contrôle de l’accès conditionnel

## Objectif

L’accès conditionnel est l’outil utilisé par Azure Active Directory pour rassembler les signaux, prendre des décisions et exécuter les politiques organisationnelles. Une politique d’accès conditionnel précise les applications ou les services que vous voulez protéger, les conditions qui régissent les applications ou les services auxquels les utilisateurs ont accès et les utilisateurs auxquels la politique s’applique. Les politiques sont exécutées après l’achèvement de l’authentification du premier facteur.

## Principales considérations

* Empêcher tout appareil non autorisé à avoir accès à des renseignements opérationnels ou personnels de nature sensible.
* Veiller à ce que les utilisateurs comprennent leurs responsabilités lorsqu’ils utilisent des appareils personnels pour avoir accès aux données et aux services et les risques d’échanger des données opérationnelles avec des utilisateurs non autorisés.
* Établir [les politiques d’accès conditionnel](https://docs.microsoft.com/fr-ca/azure/active-directory/conditional-access/overview) comme les suivantes :
  * Bloquer ou exiger l’authentification multifactorielle (MFA) pour toute tentative d’accès à partir de l’extérieur du réseau de l’entreprise
  * Exiger l’authentification multifactorielle pour les utilisateurs ayant des rôles administratifs
  * Nécessite une authentification multifactorielle pour les tâches de gestion Azure
  * Blocage des connexions pour les utilisateurs qui tentent d’utiliser les protocoles d’authentification existants
  * Exiger des emplacements de confiance pour l’enregistrement d’authentification multifactorielle Azure
  * Blocage ou octroi d’accès à partir de sites spécifiques
  * Blocage des comportements de connexion risqués
  * Exiger des dispositifs gérés par le GC pour des applications particulières en tenant compte de la catégorisation des données
* Mettre en œuvre des politiques pour surveiller et prévenir ce qui suit :
  * les utilisateurs présentant un risque;
  * les connexions à risque;
  * les détections de risques.
* Mettre en œuvre la politique d’accès conditionnel axée sur les appareils et l’état de conformité de manière à permettre ou bloquer l’accès aux applications et aux services.

## Autres considérations

* Pour les **appareils appartenant à l’organisation**, à tout le moins, veiller à ce que les configurations suivantes soient appliquées :
  * permettre l’accès au proxy d’applications Web (WAP) et aux politiques d’authentification afin de veiller à ce que l’appareil appartienne à l’organisation;
  * veiller à ce que l’AFM soit activée pour tous les comptes, y compris l’utilisation de l’application de mot de passe à usage unique.
* Pour les **appareils personnels**, à tout le moins, veiller à ce que les configurations suivantes soient appliquées :
  * veiller à ce que l’AFM soit activée pour tous les comptes, y compris l’utilisation de l’application de mot de passe à usage unique;
  * configurer les capacités de classification des données pour surveiller et protéger les données de nature sensible;
  * configurer le proxy inverse au moyen de [Microsoft Cloud App Security (MCAS)](https://docs.microsoft.com/fr-ca/cloud-app-security/proxy-intro-aad) pour protéger les données lorsque l’on utilise des navigateurs Web;
  * utiliser la [gestion des applications mobiles (MAM)](https://docs.microsoft.com/fr-ca/mem/intune/apps/mam-faq) Intune pour protéger les données dans une application. Cela comprend utiliser la MAM et les politiques de protection des applications sur les appareils qui ne sont pas inscrits à la gestion des périphériques mobiles (MDM) Intune.

## Validation

* Confirmer que des politiques d’accès conditionnel sont en place pour les appareils
* Confirmer que des politiques d’accès conditionnel sont en place pour permettre l’ACM

## Références

1. [AMOPS 2017-01](https://www.canada.ca/en/treasury-board-secretariat/services/access-information-privacy/security-identity-management/direction-secure-use-commercial-cloud-services-spin.html), section 6.2.3
2. Les 10 principales mesures de sécurité du CST, numéro 3.
3. Voir le [Guide sur l’authentification des utilisateurs dans les systèmes de technologie de l’information (ITSP.30.031 v3)](https://cyber.gc.ca/fr/orientation/guide-sur-lauthentification-des-utilisateurs-dans-les-systemes-de-technologie-de)
4. Voir [l’Orientation sur l’authentification du nuage à l’intention du gouvernement du Canada](https://intranet.canada.ca/wg-tg/cagc-angc-fra.asp)
5. Voir les [Recommandations pour l’authentification de l’utilisateur à deux facteurs au sein du domaine opérationnel du gouvernement du Canada](https://intranet.canada.ca/wg-tg/rtua-rafu-fra.asp)
6. Mesures de sécurité connexes : AC-2, AC-2(1), AC-3, AC-5, AC-6, AC-6(5), AC-6(10), AC-7, AC-9, AC-19, AC-20(3), IA-2, IA-2(1), IA-2(2), IA-2(11), IA-4, IA-5, IA-5(1), IA-5(6), IA-5(7), IA-5(13), IA-6, IA-8.
