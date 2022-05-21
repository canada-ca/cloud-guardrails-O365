# Appliquer des politiques de contrôle de l’accès conditionnel

([Retourner](/README.md#mesures-de-sécurité-initiales))

## Objectif

L’accès conditionnel est l’outil utilisé par Azure Active Directory pour rassembler les signaux, prendre des décisions et exécuter les politiques organisationnelles. Une politique d’accès conditionnel précise les applications ou les services que vous voulez protéger, les conditions qui régissent les applications ou les services auxquels les utilisateurs ont accès et les utilisateurs auxquels la politique s’applique. Les politiques sont exécutées après l’achèvement de l’authentification du premier facteur. Par exemple, des politiques visant à empêcher tout appareil non autorisé d’accéder à des renseignements commerciaux ou personnels de nature délicate devraient être envisagées.

## Principales considérations

* Veiller à ce que les utilisateurs comprennent leurs responsabilités lorsqu’ils utilisent des appareils personnels pour avoir accès aux données et aux services et les risques d’échanger des données opérationnelles avec des utilisateurs non autorisés.
* Établir des [stratégies d’accès conditionnel](https://docs.microsoft.com/fr-ca/azure/active-directory/conditional-access/overview) pour répondre aux problèmes d’accès courants comme :
  * le blocage ou l’exigence d’une authentification à facteurs multiples (AFM) pour toute tentative d’accès de l’extérieur du réseau organisationnel;
  * la demande d’authentification multifacteur pour les utilisateurs disposant de rôles d’administration;
  * la demande d’authentification multifacteur pour les tâches de gestion Azure;
  * le blocage des connexions pour les utilisateurs tentant d’utiliser des protocoles d’authentification hérités;
  * la demande d’emplacements approuvés pour l’inscription à l’authentification multifacteur Azure AD;
  * le blocage ou l’octroi de l’accès à partir d’emplacements spécifiques;
  * le blocage des comportements de connexion à risque;
  * la nécessité d’appareils gérés par le GC pour des applications précises en tenant compte de la catégorisation des données.
* Mettre en œuvre des politiques pour surveiller et prévenir ce qui suit :
  * les utilisateurs présentant un risque;
  * les connexions à risque;
  * les détections de risques.
* Mettre en œuvre la politique d’accès conditionnel axée sur les appareils et l’état de conformité de manière à permettre ou bloquer l’accès aux applications et aux services.

## Autres considérations

* Pour les **appareils appartenant à l’organisation**, envisager de mettre en œuvre les paramètres suivants :
  * permettre l’accès au proxy d’applications Web (WAP) et aux politiques d’authentification afin de veiller à ce que l’appareil appartienne à l’organisation;
  * veiller à ce que l’AFM soit activée pour tous les comptes, y compris l’utilisation de l’application de mot de passe à usage unique.
* Pour les **appareils personnels**, envisager de mettre en œuvre les paramètres suivants :
  * veiller à ce que l’AFM soit activée pour tous les comptes, y compris l’utilisation de l’application de mot de passe à usage unique;
  * étudier les capacités de classification des données pour surveiller et protéger les données de nature délicate;
  * explorer une configuration de proxy inverse à l’aide de [Microsoft Cloud App Security (MCAS)](https://docs.microsoft.com/fr-ca/defender-cloud-apps/proxy-intro-aad) pour protéger les données durant l’utilisation de navigateurs Web (licence supplémentaire requise);
  * envisager d’utiliser Intune [gestion des applications mobiles (GAM)](https://docs.microsoft.com/fr-ca/mem/intune/apps/mam-faq) pour protéger les données dans une application. Cela comprend l’utilisation de la GAM et des politiques de protection des applications sur les appareils qui ne sont pas inscrits à Intune gestion des applications mobiles (GAM).

## Validation

* Valider que des politiques d’accès conditionnel sont en place pour les appareils.
* Valider que des politiques d’accès conditionnel sont en place pour permettre la GAM.

## Références

1. [Directive sur la gestion de la sécurité, annexe B : Procédures obligatoires relatives aux mesures de sécurité de la technologie de l’information](https://www.tbs-sct.canada.ca/pol/doc-fra.aspx?id=32611), sous-sections B.2.3.1 et B.2.3.2.4.
2. [AMOPS 2017-01](https://www.canada.ca/en/treasury-board-secretariat/services/access-information-privacy/security-identity-management/direction-secure-use-commercial-cloud-services-spin.html), section 6.2.3.
3. Les 10 principales mesures de sécurité du CST, numéro 3.
4. Voir le [Guide sur l’authentification des utilisateurs dans les systèmes de technologie de l’information (ITSP.30.031 v3) du CCC](https://cyber.gc.ca/fr/orientation/guide-sur-lauthentification-des-utilisateurs-dans-les-systemes-de-technologie-de).
5. Voir l'[Orientation sur l’authentification du nuage à l’intention du gouvernement du Canada](https://intranet.canada.ca/wg-tg/cagc-angc-fra.asp).
6. Voir les [Recommandations pour l’authentification de l’utilisateur à deux facteurs au sein du domaine opérationnel du gouvernement du Canada](https://intranet.canada.ca/wg-tg/rtua-rafu-fra.asp).
7. Mesures de sécurité connexes : AC-2, AC-2(1), AC-3, AC-5, AC-6, AC-6(5), AC-6(10), AC-7, AC-9, AC-19, AC-20(3), IA-2, IA-2(1), IA-2(2), IA-2(11), IA-4, IA-5, IA-5(1), IA-5(6), IA-5(7), IA-5(13), IA-6, IA-8.
