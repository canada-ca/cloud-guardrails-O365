# Exécuter le renforcement des services

## Objectif

Réduire au minimum les services disponibles et contrôler la connectivité en désactivant les services ainsi que les comptes inutiles des systèmes. Configurer le service Office 365 et les appareils qui y ont accès pour tenter de filtrer et de réduire l’impact des tentatives d’attaque.

## Principales considérations

* [ ] Configurer les paramètres de collaboration externe.
* [ ] Configurer Azure Information Protection.
* [ ] Veiller à ce que O365 ATP SafeLinks pour les applications Office soit activé.
* [ ] Désactiver les macros lorsqu’elles ne sont pas utilisées.
* [ ] Désactiver les capacités de macro à risque élevé.
* [ ] Configurer la détection de l’exécution des macros.
* [ ] Désactivez les macros à moins qu’elles ne se trouvent dans des fichiers de confiance – Fichiers de confiance (signature ou emplacement).
* [ ] Bloquer les macros d’Internet.
* [ ] Configurer la [protection contre les programmes malveillants](https://docs.microsoft.com/fr-ca/microsoft-365/security/office-365-security/anti-malware-protection?view=o365-worldwide) sur le client.
* [ ] Examiner les permissions accordées aux services tiers au moyen des Applications intégrées.

### Teams

* [ ] Veiller à ce que les utilisateurs comprennent la catégorisation du site Teams (p. ex., les sites Teams peuvent être approuvés seulement pour les renseignements non classifiés).
* [ ] Veiller à ce que les utilisateurs comprennent leurs responsabilités pour gérer l’information, y compris les décisions d’enregistrement prises dans le répertoire de GI ministériel.
* [ ] Les responsables de sites Teams sont responsables de gérer leurs groupes Office 365 qui sont les groupes de mesures de contrôle de l’accès de sécurité afin de permettre l’accès au site Teams.
* [ ] S’assurer d’examiner les applications Microsoft, les applications de tiers et les applications client que votre organisation autorisera dans Teams.
* [ ] Désactiver l’accès externe à moins que votre organisation doive collaborer avec les utilisateurs externes.
* [ ] Désactiver l’accès invité à moins que votre organisation doive collaborer avec des invités.
* [ ] Désactiver les services de partage de fichiers (ShareFile, Dropbox, Box, Google Drive) si leur utilisation n’a pas été approuvée dans votre organisation.

### Exchange Online

* [ ] Veiller à ce que l’authentification moderne pour Exchange Online soit activée.
* [ ] Veiller à ce que le [filtre des types communs de fichiers joints](https://docs.microsoft.com/fr-ca/exchange/security-and-compliance/mail-flow-rules/common-attachment-blocking-scenarios) soit activé.
* [ ] Veiller à ce que les règles de transport des courriels [n’acheminent pas](https://docs.microsoft.com/fr-ca/microsoft-365/admin/security-and-compliance/secure-your-business-data?view=o365-worldwide#forwarding) les courriels à des domaines externes.
* [ ] Veiller à ce que les règles de transport des courriels n’inscrivent pas des domaines particuliers à la liste blanche.
* [ ] Veiller à ce qu’une [politique contre l’hameçonnage](https://docs.microsoft.com/fr-ca/microsoft-365/admin/security-and-compliance/secure-your-business-data?view=o365-worldwide#8-protect-your-email-from-phishing-attacks) ait été créée.
* [ ] Veiller à ce que les avertissements aux utilisateurs internes qui envoient des logiciels malveillants soient activés.
* [ ] Veiller à ce que la politique [Advanced Threat Protection SafeLinks](https://docs.microsoft.com/fr-ca/microsoft-365/admin/security-and-compliance/secure-your-business-data?view=o365-worldwide#10-protect-against-phishing-attacks-with-atp-safe-links) soit activée.
* [ ] Désactiver les services inutilisés par boîte de courriels.
* [ ] Configurer la règle de transport concernant les [rançongiciels](https://docs.microsoft.com/fr-ca/microsoft-365/admin/security-and-compliance/secure-your-business-data?view=o365-worldwide#ransomware) pour bloquer les extensions de fichier qui sont communément utilisées pour les rançongiciels ou pour avertir les utilisateurs qui reçoivent ces fichiers joints dans leurs courriels.
* [ ] Autoriser toutes les adresses IP qui transmettent des données dans le Sender Policy Framework (SPF) et veiller à ce que DKIM soit activé pour tous les domaines Exchange Online.
* [ ] Appliquer les signatures Domain Keys Identified Mail (DKIM) à tous les messages expédiés pour tous les domaines Exchange Online.
* [ ] Établir une politique minimum de Domain-based Message Authentication, Reporting & Conformance (DMARC) de « p=none » avec au moins une adresse définie comme destinataire des rapports agrégés, conformément au guide de mise en œuvre pour la protection des domaines de courriels du CCC.
* [ ] Ajouter le Centre canadien pour la cybersécurité (CCC) comme destinataire du rapport agrégé dans les dossiers DMARC. L’adresse à inclure est [dmarc@cyber.gc.ca](mailto:dmarc@cyber.gc.ca).

## Autres considérations

* [ ] Utiliser le [chiffrement des messages Office](https://docs.microsoft.com/fr-ca/microsoft-365/admin/security-and-compliance/secure-your-business-data?view=o365-worldwide#7-use-office-message-encryption) pour offrir des options de protection pour l’envoi de courriels marqués « Ne pas transférer » ou « Chiffrer ».
* [ ] Considérer l’activation de la politique [Pièces jointes fiables Advanced Threat Protection](https://docs.microsoft.com/fr-ca/microsoft-365/admin/security-and-compliance/secure-your-business-data?view=o365-worldwide#9-protect-against-malicious-attachments-and-files-with-atp-safe-attachments).
* [ ] Dans la mesure du possible, utiliser le traitement des incidences et la résolution des menaces O365 automatisés.
* [ ] Activer les services de renseignements sur les menaces afin d’aider à renforcer la fonction Advanced Threat Protection d’O365.
* [ ] Augmenter la surveillance et le contrôle de l’environnement d’informatique en nuage en utilisant des services comme des courtiers de sécurité d’accès au nuage (CASB) et des services d’analyse du comportement des utilisateurs et des entités (UEBA).
* [ ] S’assurer que les mises à jour et les fonctions du produit sont examinées et configurées au fur et à mesure de leur disponibilité et, le cas échéant

## Validation

* [ ] À déterminer

## Références

1. [AMOPS 2017-01](https://www.canada.ca/en/treasury-board-secretariat/services/access-information-privacy/security-identity-management/direction-secure-use-commercial-cloud-services-spin.html), section 6.2.3.
2. Les 10 principales mesures de sécurité du CST, numéro 3.
3. Voir le [Guide sur l’authentification des utilisateurs dans les systèmes de technologie de l’information (ITSP.30.031 v3) du CCC](https://cyber.gc.ca/fr/orientation/guide-sur-lauthentification-des-utilisateurs-dans-les-systemes-de-technologie-de)
4. Voir [l’Orientation sur l’authentification du nuage à l’intention du gouvernement du Canada](https://intranet.canada.ca/wg-tg/cagc-angc-fra.asp)
5. Voir les [Recommandations pour l’authentification de l’utilisateur à deux facteurs au sein du domaine opérationnel du gouvernement du Canada](https://intranet.canada.ca/wg-tg/rtua-rafu-fra.asp)
6. Mesures de sécurité connexes : AC-2, AC-2(1), AC-3, AC-5, AC-6, AC-6(5), AC-6(10), AC-7, AC-9, AC-19, AC-20(3), IA-2, IA-2(1), IA-2(2), IA-2(11), IA-4, IA-5, IA-5(1), IA-5(6), IA-5(7), IA-5(13), IA-6, IA-8.
