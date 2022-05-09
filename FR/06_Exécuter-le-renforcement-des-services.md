# Exécuter le renforcement des services

## Objectif

Réduire au minimum les services disponibles et contrôler la connectivité en désactivant les services ainsi que les comptes inutiles des systèmes. Configurer le service Office 365 et les appareils qui y ont accès pour tenter de filtrer et de réduire l’impact des tentatives d’attaque.

## Principales considérations

* Configurer les paramètres de collaboration externe.
* Configurer Azure Information Protection.
* Veiller à ce qu’O365 ATP SafeLinks pour les applications Office soit activé.
* Désactiver les macros lorsqu’elles ne sont pas utilisées.
* Désactiver les capacités de macro à risque élevé.
* Configurer la détection de l’exécution des macros.
* Désactiver les macros à moins qu’elles ne se trouvent dans des fichiers de confiance – Fichiers de confiance (signature ou emplacement).
* Bloquer les macros d’Internet.
* Configurer la [protection contre les programmes malveillants](https://docs.microsoft.com/fr-ca/microsoft-365/security/office-365-security/anti-malware-protection?view=o365-worldwide) sur le client.
* Veiller à ce que les applications intégrées tierces ne soient pas autorisées.

### Teams

* Veiller à ce que les utilisateurs comprennent la catégorisation du site Teams (p. ex., les sites Teams peuvent être approuvés seulement pour les renseignements non classifiés).
* Veiller à ce que les utilisateurs comprennent leurs responsabilités pour gérer l’information, y compris les décisions d’enregistrement prises dans le répertoire de gestion de l’information ministériel.
* Les responsables de sites Teams sont responsables de gérer leurs groupes Office 365 qui sont les groupes de contrôles de l’accès de sécurité afin de permettre l’accès au site Teams.
* S’assurer d’examiner les applications Microsoft, les applications de tiers et les applications client que votre organisation autorisera dans Teams.
* Désactiver l’accès externe à moins que votre organisation doive collaborer avec les utilisateurs externes. Configurer des stratégies d’accès externes pour activer la collaboration avec les domaines approuvés.
* Désactiver l’accès invité à moins que votre organisation l’exige. Limiter le nombre d’utilisateurs invités dans l’environnement, en veillant à ce que la politique et les procédures d’accès des utilisateurs invités soient conformes à la politique et aux procédures définies dans la mesure de protection [Gérer l’identité et l’accès](https://canada-ca.github.io/cloud-guardrails-O365/FR/01_Manage-Identity-Access.html).
* Désactiver les services de partage de fichiers (ShareFile, Dropbox, Box, Google Drive) si leur utilisation n’a pas été approuvée dans votre organisation.

### Exchange Online

* Veiller à ce que l’authentification moderne pour Exchange Online soit activée.
* Veiller à ce que les détails du calendrier partagés avec des utilisateurs externes soient désactivés.
* Configurer le filtrage des connexions.
* Veiller à ce que les politiques antipourriel et de protection d’Exchange Online soient configurées correctement.
* Veiller à ce que le [filtre des types de pièces jointes courants](https://docs.microsoft.com/fr-ca/exchange/security-and-compliance/mail-flow-rules/common-attachment-blocking-scenarios) soit activé pour la [protection anti-programme malveillant](https://docs.microsoft.com/fr-ca/microsoft-365/security/office-365-security/anti-malware-protection?view=o365-worldwide).
* Veiller à ce que les règles de transport des courriels [n’acheminent pas](https://docs.microsoft.com/fr-ca/microsoft-365/admin/security-and-compliance/secure-your-business-data?view=o365-worldwide) les courriels à des domaines externes.
* Veiller à ce que les règles de transport des courriels n’inscrivent pas des domaines particuliers à la liste blanche.
* Veiller à ce qu’une [politique contre l’hameçonnage](https://docs.microsoft.com/fr-ca/microsoft-365/admin/security-and-compliance/secure-your-business-data?view=o365-worldwide) ait été créée.
* Veiller à ce que les avertissements aux utilisateurs internes qui envoient des logiciels malveillants soient activés.
* Veiller à ce que la politique de [liens Coffre pour protection avancée contre les menaces](https://docs.microsoft.com/fr-ca/microsoft-365/admin/security-and-compliance/secure-your-business-data?view=o365-worldwide) soit activée.
* Désactiver les services inutilisés par boîte de courriels.
* Configurer la règle de transport concernant les rançongiciels pour bloquer les extensions de fichier qui sont communément utilisées pour les rançongiciels ou pour avertir les utilisateurs qui reçoivent ces fichiers joints dans leurs courriels.
* Autoriser toutes les adresses IP qui transmettent des données dans le Sender Policy Framework (SPF) et veiller à ce que DKIM soit activé pour tous les domaines Exchange Online.
* Appliquer les signatures Domain Keys Identified Mail (DKIM) à tous les messages expédiés pour tous les domaines Exchange Online.
* Établir une politique minimum de Domain-based Message Authentication, Reporting & Conformance (DMARC) de « p=none » avec au moins une adresse définie comme destinataire des rapports agrégés, conformément au guide de mise en œuvre pour la protection des domaines de courriels du CCC.
* Ajouter le Centre canadien pour la cybersécurité (CCC) comme destinataire du rapport agrégé dans les dossiers DMARC. L’adresse à inclure est dmarc@cyber.gc.ca.

## Autres considérations

* Utiliser [Office chiffrement des messages](https://docs.microsoft.com/fr-ca/microsoft-365/admin/security-and-compliance/secure-your-business-data?view=o365-worldwide) pour offrir des options de protection pour l’envoi de courriels marqués « Ne pas transférer » ou « Chiffrer ».
* Considérer l’activation de la [politique de pièces jointes Coffre pour protection avancée contre les menaces](https://docs.microsoft.com/fr-ca/microsoft-365/admin/security-and-compliance/secure-your-business-data?view=o365-worldwide).
* Dans la mesure du possible, utiliser le traitement des incidences et la résolution des menaces O365 automatisés.
* Explorer l’utilisation des services de renseignements sur les menaces afin d’aider à renforcer la fonction Advanced Threat Protection d’O365.
* Considérer une surveillance et un contrôle de l’environnement d’informatique en nuage accrus en utilisant des services comme un courtier de sécurité d’accès au nuage (CASB) et des services d’analyse du comportement des utilisateurs et des entités (UEBA).
* Veiller à ce que les mises à jour et les fonctionnalités du produit soient examinées et configurées au fur et à mesure qu’elles deviennent disponibles et selon le besoin.

## Validation

* À déterminer

## Références

1. [Directive sur la gestion de la sécurité, annexe B : Procédures obligatoires relatives aux mesures de sécurité de la technologie de l’information](https://www.tbs-sct.canada.ca/pol/doc-fra.aspx?id=32611), sous-sections B.2.3.3 et B.2.3.7.
2. [AMOPS 2017-01](https://www.canada.ca/en/treasury-board-secretariat/services/access-information-privacy/security-identity-management/direction-secure-use-commercial-cloud-services-spin.html), section 6.2.3.
3. Les 10 principales mesures de sécurité du CST, numéro 3.
4. Voir le [Guide sur l’authentification des utilisateurs dans les systèmes de technologie de l’information (ITSP.30.031 v3) du CCC](https://cyber.gc.ca/fr/orientation/guide-sur-lauthentification-des-utilisateurs-dans-les-systemes-de-technologie-de)
5. Voir l'[Orientation sur l’authentification du nuage à l’intention du gouvernement du Canada](https://intranet.canada.ca/wg-tg/cagc-angc-fra.asp)
6. Voir les [Recommandations pour l’authentification de l’utilisateur à deux facteurs au sein du domaine opérationnel du gouvernement du Canada](https://intranet.canada.ca/wg-tg/rtua-rafu-fra.asp)
7. Mesures de sécurité connexes : AC-2, AC-2(1), AC-3, AC-5, AC-6, AC-6(5), AC-6(10), AC-7, AC-9, AC-19, AC-20(3), IA-2, IA-2(1), IA-2(2), IA-2(11), IA-4, IA-5, IA-5(1), IA-5(6), IA-5(7), IA-5(13), IA-6, IA-8.
