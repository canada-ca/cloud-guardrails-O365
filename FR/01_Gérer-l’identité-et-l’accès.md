# Gérer l’identité et l’accès

## Objectif

Gérer les identités et établir des stratégies et des procédures de contrôle d’accès pour la gestion des privilèges d’administration.

## Principales considérations

### Identité

* [ ] Empêcher l’utilisation d’anciens protocoles d’authentification.
* [ ] Activer la protection de l’identité.
* [ ] Configurer la protection par mot de passe d’Azure AD.
* [ ] Tirer profit de l’authentification fédérée, si disponible.
* [ ] Configurer ADFS pour utiliser Azure MFA comme principal mécanisme d’authentification.
* [ ] Configurer ADFS pour bloquer les anciennes authentifications à partir de l’extranet.
* [ ] Configurer le verrouillage de l’extranet au proxy d’applications Web.
* [ ] Configurer les comptes d’urgence dans Azure AD.

### Accès

* [ ]  Mettre en œuvre un mécanisme pour identifier et authentifier de façon unique les utilisateurs organisationnels, les utilisateurs non organisationnels (le cas échéant) et les processus (p. ex., nom d’utilisateur et mot de passe).
* [ ]  Veiller à ce que l’authentification à facteurs multiples soit activée pour tous les utilisateurs occupant des rôles d’administrateur.
* [ ]  Veiller à ce que de deux à quatre administrateurs généraux soient nommés.
* [ ]  Mettre en œuvre l’accès fondé sur les rôles et utiliser les rôles avec le moins de privilèges dans la mesure du possible (p. ex., utiliser des rôles d’administrateur non général).
* [ ]  Configurer l’accès juste-à-temps pour permettre un accès privilégié au fur et à mesure des besoins.*
* [ ]  Configurer les membres du rôle d’administrateur général d’Office 365.
* [ ]  Utiliser des comptes dédiés pour exécuter les tâches administratives.
* [ ]  Veiller à ce que l’authentification moderne pour les applications SharePoint soit requise.
* [ ]  Veiller à ce que l’authentification moderne pour Skype for Business Online soit activée.
* [ ]  Veiller à ce que l’authentification moderne pour Exchange Online soit activée.
* [ ]  Configurer la politique sur les mots de passe conformément à [l’Orientation sur les mots de passe du GC](https://www.canada.ca/fr/gouvernement/systeme/gouvernement-numerique/orientation-sur-mots-passe.html).
* [ ]  Réduire au minimum le nombre d’utilisateurs invités; ajouter uniquement au besoin.
* [ ]  Veiller à ce que les [restrictions des locataires](https://docs.microsoft.com/en-us/azure/active-directory/manage-apps/tenant-restrictions) soient configurées
* [ ] Examiner régulièrement les rapports sur l’accès pour tous les comptes d’administrateur et les rapports, conformément à [Activer la journalisation et la surveillance](04_Activer-la-journalisation-et-la-surveillance.md) mesures de sécurité

## Autres considérations

* [ ] Déterminer les restrictions d’accès et les exigences de configuration pour les dispositifs d’extrémité délivrés par le GC, y compris ceux des utilisateurs privilégiés et non privilégiés, et configurer les restrictions d’accès pour les dispositifs d’extrémité en conséquence
* [ ] Configurer l’accès juste-à-temps pour permettre l’accès administratif au besoin
* [ ] Limiter la divulgation de renseignements de nature délicate du GC au personnel de soutien. Si l’accès aux données est requis, tirer parti de la fonction de boîte à serrure du client.

## Validation

* [ ] Confirmer qu’un plan et un processus de gestion des comptes privilégiés ont été consignés.
* [ ] Confirmer que la politique sur les mots de passe respecte [l’Orientation sur les mots de passe du GC](https://www.canada.ca/fr/gouvernement/systeme/gouvernement-numerique/orientation-sur-mots-passe.html), le cas échéant.

## Références

1. [AMOPS 2017-01](https://www.canada.ca/en/treasury-board-secretariat/services/access-information-privacy/security-identity-management/direction-secure-use-commercial-cloud-services-spin.html), section 6.2.3
2. Les 10 principales mesures de sécurité du CST, numéro 3.
3. Voir le [Guide sur l’authentification des utilisateurs dans les systèmes de technologie de l’information (ITSP.30.031 v3)](https://cyber.gc.ca/fr/orientation/guide-sur-lauthentification-des-utilisateurs-dans-les-systemes-de-technologie-de)
4. Voir [l’Orientation sur l’authentification du nuage à l’intention du gouvernement du Canada](https://intranet.canada.ca/wg-tg/cagc-angc-fra.asp) *_(accessible seulement sur le réseau du gouvernement du Canada)_*
5. Voir les [Recommandations pour l’authentification de l’utilisateur à deux facteurs au sein du domaine opérationnel du gouvernement du Canada](https://intranet.canada.ca/wg-tg/rtua-rafu-fra.asp) *_(accessible seulement sur le réseau du gouvernement du Canada)_*
6. Mesures de sécurité connexes : AC-2, AC-2(1), AC-3, AC-5, AC-6, AC-6(5), AC-6(10), AC-7, AC-9, AC-19, AC-20(3), IA-2, IA-2(1), IA-2(2), IA-2(11), IA-4, IA-5, IA-5(1), IA-5(6), IA-5(7), IA-5(13), IA-6, IA-8.
