# GC Cloud Guardrails for O365

([Français](#mesures-de-sécurité-dinformatique-en-nuage-du-gc-pour-o365))

This project will host the minimum guardrails for Microsoft Office 365. The users of this project will be Government of Canada employees deploying cloud-based workloads.

## Purpose

The purpose of the guardrails is to ensure that departments and agencies are implementing a preliminary baseline set of controls within their Microsoft O365 cloud-based environment.

## Initial Guardrails

A summary of the cloud guardrails to be implemented in the initial phase are identified in the table below.

| ID. | Guardrail                                                               |
| --- | ----------------------------------------------------------------------- |
| 01  | [Manage identity and access](EN/01_Manage-Identity-Access.md)           |
| 02  | [Use multi-factor authentication](EN/02_Use-MFA.md)                     |
| 03  | [Apply conditional access policies](EN/03_Apply-Conditional-Access.md)  |
| 04  | [Enable logging and monitoring](EN/04_Enable-Logging-and-Monitoring.md) |
| 05  | [Implement data protection](EN/05_Implement-Data-Protection.md)         |
| 06  | [Perform service hardening](EN/06_Perform-Service-Hardening.md)         |
| 07  | [Perform device hardening](EN/07_Perform-Device-Hardening.md)           |
| 08  | [Validate settings](EN/08_Validate-Settings.md)                         |

**_DRAFT detailed implementation guidance is to implement the guardrails is available on [GCpedia](https://www.gcpedia.gc.ca/gcwiki/images/d/d9/Microsoft_365_Security_Baseline_Configuration_ver_2.3.xlsx) (accessible only on the Government of Canada network). Please note that this is a living document and subject to change as new services and features are made available._**

Departments should consider using [Microsoft Secure Score](https://docs.microsoft.com/en-us/microsoft-365/security/mtp/microsoft-secure-score?view=o365-worldwide) when starting their configuration. Secure Score is a measurement of an organization's security posture, with a higher number indicating more improvement actions taken. It provides recommendations and guidance that can protect the organization from threats.

### Considerations

Departments are expected to continue implementing the security requirements as outlined in:

- [Direction on the Secure Use of Commercial Cloud Services: Security Implementation Notice (SPIN)](https://www.canada.ca/en/government/system/digital-government/modern-emerging-technologies/direction-secure-use-commercial-cloud-services-spin.html)
- [Government of Canada Security Control Profile for Cloud-Based GC Services](https://www.canada.ca/en/government/system/digital-government/modern-emerging-technologies/cloud-services/government-canada-security-control-profile-cloud-based-it-services.html)

Departments should engage with their IT Security Risk Management teams to obtain advice and guidance on integrating security assessment and authorization activities as part of the implementation of the GC cloud environment. The [Government of Canada Cloud Security Risk Management Approach and Procedures](https://www.canada.ca/en/government/system/digital-government/digital-government-innovations/cloud-services/cloud-security-risk-management-approach-procedures.html) outlines activities for Departments to consider as part of the departmental risk management activities.

### How to Contribute

See [CONTRIBUTING.md](CONTRIBUTING.md)

### License

Unless otherwise noted, the source code of this project is covered under Crown Copyright, Government of Canada, and is distributed under the [MIT License](LICENSE).

The Canada wordmark and related graphics associated with this distribution are protected under trademark law and copyright law. No permission is granted to use them outside the parameters of the Government of Canada's corporate identity program. For more information, see [Federal identity requirements](https://www.canada.ca/en/treasury-board-secretariat/topics/government-communications/federal-identity-requirements.html).

---

<!-- markdownlint-disable MD024 MD025 -->

# Mesures de sécurité d’informatique en nuage du GC pour O365

Ce projet hébergera les mesures de sécurité minimales pour Microsoft Office 365. Les utilisateurs de ce projet seront des employés du gouvernement du Canada qui déploient des charges de travail dans le nuage.

## But

Le but des mesures de sécurité est de veiller à ce que les ministères et les organismes mettent en œuvre un ensemble préliminaire de mesures dans leur propre environnement d’informatique en nuage pour Microsoft O365.

## Mesures de sécurité initiales

Un résumé des mesures de sécurité d’informatique en nuage à mettre en œuvre dans le cadre de la phase initiale est fourni dans le tableau ci-dessous :

| ID. | Mesures de sécurité du nuage                                                                            |
| --- | ------------------------------------------------------------------------------------------------------- |
| 01  | [Gérer l’identité et l’accès](FR/01_Gérer-l’identité-et-l’accès.md)                                     |
| 02  | [Utiliser l’authentification à facteurs multiples](FR/02_Utiliser-AFM.md)                               |
| 03  | [Appliquer des politiques d’accès conditionnel](FR/03_Appliquer-des-politiques-d’accès-conditionnel.md) |
| 04  | [Activer la journalisation et la surveillance](FR/04_Activer-la-journalisation-et-la-surveillance.md)   |
| 05  | [Mettre en œuvre la protection des données](FR/05_Mettre-en-œuvre-la-protection-des-données.md)         |
| 06  | [Exécuter le renforcement des services](FR/06_Exécuter-le-renforcement-des-services.md)                 |
| 07  | [Exécuter le renforcement des appareils](FR/07_Exécuter-le-renforcement-des-appareils.md)               |
| 08  | [Valider les paramètres](FR/08_Valider-les-paramètres.md)                                               |

**_L’ÉBAUCHE du guide de mise en œuvre détaillé pour mettre en œuvre les mesures de sécurité est disponible à partir du site [GCpedia](https://www.gcpedia.gc.ca/gcwiki/images/0/0b/Office_365_Security_Baseline_Configuration.xlsx) (accessible uniquement par l’entremise du réseau du gouvernement du Canada). Veuillez prendre note qu’il s’agit d’un document constamment modifié assujetti au changement au fur et à mesure que de nouveaux services et de nouvelles fonctionnalités sont offerts._**

Les ministères devraient envisager d’utiliser [Degré de sécurisation Microsoft](https://docs.microsoft.com/fr-fr/microsoft-365/security/mtp/microsoft-secure-score?view=o365-worldwide) au début de leur configuration. Degré de sécurisation est une mesure de la posture de sécurité d’une organisation, avec un plus grand nombre indiquant plus de mesures d’amélioration prises. Il fournit des recommandations et des directives qui peuvent protéger l’organisation contre les menaces.

## Considerations

Les ministères devraient continuer à mettre en œuvre les exigences de sécurité énoncées dans les documents suivants :

- [Orientation sur l’utilisation sécurisée des services commerciaux d’informatique en nuage : Avis de mise en œuvre de la Politique sur la sécurité (AMOPS)](https://www.canada.ca/fr/gouvernement/systeme/gouvernement-numerique/technologiques-modernes-nouveaux/orientation-utilisation-securisee-services-commerciaux-informatique-nuage-amops.html)
- [Profil des mesures de sécurité pour les services du GC fondés sur l’informatique en nuage - Canada.ca](https://www.canada.ca/fr/gouvernement/systeme/gouvernement-numerique/innovations-gouvernementales-numeriques/services-informatique-nuage/profil-controle-securite-services-ti-fondes-information-nuage.html)

Les ministères devraient collaborer avec leurs équipes de gestion des risques de sécurité de la TI pour obtenir des conseils et une orientation sur l’intégration des activités d’évaluation et d’autorisation de la sécurité dans le cadre de la mise en œuvre de l’environnement de l’informatique en nuage du GC. [L’approche et les procédures de gestion des risques à la sécurité de l’informatique en nuage du gouvernement du Canada](https://www.canada.ca/fr/gouvernement/systeme/gouvernement-numerique/innovations-gouvernementales-numeriques/services-informatique-nuage/approche-procedures-gestion-risques-securite-informatique-nuage.html) décrivent les activités que les ministères doivent envisager dans le cadre des activités de gestion des risques ministériels.

### Comment contribuer

Voir [CONTRIBUTING.md](CONTRIBUTING.md)

### Licence

Sauf indication contraire, le code source de ce projet est protégé par le droit d’auteur de la Couronne du gouvernement du Canada et distribué sous la [licence MIT](LICENSE).

Le mot-symbole « Canada » et les éléments graphiques connexes liés à cette distribution sont protégés en vertu des lois portant sur les marques de commerce et le droit d’auteur. Aucune autorisation n’est accordée pour leur utilisation à l’extérieur des paramètres du programme de coordination de l’image de marque du gouvernement du Canada. Pour obtenir de plus amples renseignements à ce sujet, veuillez consulter les [Exigences pour l’image du Canada](https://www.canada.ca/fr/secretariat-conseil-tresor/sujets/communications-gouvernementales/exigences-image-marque.html).
