# Gérer l’identité et l’accès

## Objectif

Gérer les identités et établir des stratégies et des procédures de contrôle d’accès pour la gestion des privilèges d’administration.

## Principales considérations

### Identité

* Empêcher l’utilisation d’anciens protocoles d’authentification.
* Configurer la protection de mot de passe d’Azure AD conformément à la [Stratégie de mise en œuvre pour l’orientation sur les mots de passe du GC](https://www.gcpedia.gc.ca/gcwiki/images/c/c0/Implementation_Strategy_for_GC_Password_Guidance.pdf) (accessible uniquement sur le réseau du gouvernement du Canada).
* Configurer les comptes d’urgence dans Azure AD.
* Tirer profit de l’authentification fédérée, si disponible.
Si vous utilisez Active Directory Federation Service (ADFS), tenez compte des éléments suivants :
* Configurer ADFS pour utiliser l’authentification multifacteur Azure comme principal mécanisme d’authentification.
* Configurer ADFS pour bloquer les anciennes authentifications à partir de l’extranet.
* Configurer le verrouillage de l’extranet au proxy d’applications Web ADFS.
* Installer le certificat approuvé sur le serveur ADFS.
* Mettre en place des paramètres de sécurité supplémentaires dans ADFS pour limiter les attaques de l’intercepteur.

### Accès

* Mettre en œuvre un mécanisme pour identifier et authentifier de façon unique les utilisateurs organisationnels, les utilisateurs non organisationnels (le cas échéant) et les processus (p. ex., nom d’utilisateur et mot de passe).
* Veiller à ce que l’authentification à facteurs multiples soit activée pour tous les utilisateurs occupant des rôles d’administrateur.
* Veiller à ce que de deux à quatre administrateurs généraux soient nommés.
* Mettre en œuvre l’accès fondé sur les rôles et utiliser les rôles avec le moins de privilèges dans la mesure du possible (p. ex., utiliser des rôles d’administrateur non général).
* Configurer les membres du rôle d’administrateur général d’Office 365.
* Utiliser des comptes dédiés pour exécuter les tâches administratives.
* Contrôler l’accès au portail d’administration d’Azure AD.
* Veiller à ce que l’authentification moderne pour les applications SharePoint soit requise.
* Veiller à ce que l’authentification moderne pour Teams (anciennement Skype for Business Online) soit activée.
* Veiller à ce que l’authentification moderne pour Exchange Online soit activée.
* Configurer la politique sur les mots de passe conformément à [l’Orientation sur les mots de passe du GC](https://www.canada.ca/fr/gouvernement/systeme/gouvernement-numerique/orientation-sur-mots-passe.html).
* Désactiver l’accès utilisateur invité par défaut. Ajouter uniquement le nombre minimal de comptes, si nécessaire, conformément à une politique et à des procédures approuvées pour les utilisateurs invités, tout en veillant à ce qu’un [environnement de partage d’invités sécurisé](https://docs.microsoft.com/fr-ca/microsoft-365/solutions/create-secure-guest-sharing-environment?view=o365-worldwide) ait été établi.
* Revoir régulièrement les rapports pour tous les comptes administratifs et les rapports d’accès, conformément à la procédure de protection [Activer la journalisation et la surveillance](https://canada-ca.github.io/cloud-guardrails-O365/FR/04_Enable-Logging-and-Monitoring.html).

## Autres considérations

* Envisager d’activer la protection de l’identité (licence supplémentaire requise).
* Envisager de contrôler les tâches administratives avec une gestion d’accès privilégié (licence supplémentaire requise).
* Étudier l’accès juste à temps pour permettre l’accès administratif, au besoin (licence supplémentaire requise).
* Limiter la divulgation de renseignements confidentiels du gouvernement du Canada (GC) au personnel de soutien. Si l’accès aux données est nécessaire, utiliser la fonction « customer lockbox » (licence supplémentaire requise).
* Déterminer les exigences en matière de restrictions et de configuration d’accès pour les appareils de point d’extrémité fournis par le GC, y compris ceux des utilisateurs privilégiés et non privilégiés, et configurer en conséquence les restrictions d’accès.

## Validation

* Confirmer qu’un plan et un processus de gestion des comptes privilégiés ont été consignés.
* Confirmer que la politique sur le mot de passe est conforme à l’[orientation sur les mots de passe du GC](https://www.canada.ca/fr/government/system/digital-government/password-guidance.html) (accessible uniquement sur le réseau du gouvernement du Canada), selon le besoin.

## Références

1. [Directive sur la gestion de la sécurité, annexe B : Procédures obligatoires relatives aux mesures de sécurité de la technologie de l’information](https://www.tbs-sct.canada.ca/pol/doc-fra.aspx?id=32611) sous-sections B.2.3.1 et B.2.3.2.4.
2. [AMOPS 2017-01](https://www.canada.ca/en/treasury-board-secretariat/services/access-information-privacy/security-identity-management/direction-secure-use-commercial-cloud-services-spin.html), section 6.2.3
3. Les 10 principales mesures de sécurité du CST, numéro 3.
4. Voir le [Guide sur l’authentification des utilisateurs dans les systèmes de technologie de l’information (ITSP.30.031 v3)](https://cyber.gc.ca/fr/orientation/guide-sur-lauthentification-des-utilisateurs-dans-les-systemes-de-technologie-de)
5. Voir [l’Orientation sur l’authentification du nuage à l’intention du gouvernement du Canada](https://intranet.canada.ca/wg-tg/cagc-angc-fra.asp) (accessible seulement sur le réseau du gouvernement du Canada)
6. Voir les [Recommandations pour l’authentification de l’utilisateur à deux facteurs au sein du domaine opérationnel du gouvernement du Canada](https://intranet.canada.ca/wg-tg/rtua-rafu-fra.asp) (accessible seulement sur le réseau du gouvernement du Canada)
7. Mesures de sécurité connexes : AC-2, AC-2(1), AC-3, AC-5, AC-6, AC-6(5), AC-6(10), AC-7, AC-9, AC-19, AC-20(3), IA-2, IA-2(1), IA-2(2), IA-2(11), IA-4, IA-5, IA-5(1), IA-5(6), IA-5(7), IA-5(13), IA-6, IA-8.
