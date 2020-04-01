# Mettre en œuvre la protection des données

## Objectif

Protéger les renseignements et les actifs hébergés dans le nuage de l’accès, de l’utilisation, de la divulgation, de la modification, de l’élimination, de la transmission ou de la destruction non autorisés tout au long de leur cycle de vie.

## Principales considérations

* [ ] Demander des conseils aux responsables de la protection des renseignements personnels et de l’accès à l’information dans les institutions avant de stocker des renseignements personnels dans les environnements d’informatique en nuage.
* [ ] Vérifier l’emplacement du service, conformément à la section 4.4.1.10 de la [Directive sur les services et le numérique](https://www.tbs-sct.gc.ca/pol/doc-fra.aspx?id=32601).
* [ ] Veiller à ce que les données en transit soient chiffrées par défaut (p. ex., TLS v1.2).
  Appliquer les mécanismes de chiffrement pour protéger la confidentialité et l’intégrité des données hébergées dans le service d’informatique en nuage.
* [ ] Utiliser les algorithmes et les protocoles cryptographiques approuvés par le Centre de la sécurité des télécommunications Canada (CSTC), conformément aux publications [40.111](https://cyber.gc.ca/fr/orientation/algorithmes-cryptographiques-pour-linformation-non-classifie-protege-et-protege-b) et [40.062](https://www.cse-cst.gc.ca/en/system/files/pdf_documents/itsp.40.062-eng.pdf).
* [ ] Activer les politiques de prévention de la perte de données au niveau du service d’informatique en nuage afin de permettre au contenu sur Exchange Online et SharePoint Online d’être analysé pour des types particuliers de données comme les numéros de sécurité sociale, les numéros de carte de crédit ou les mots de passe.
* [ ] Tirer profit de la Gouvernance des données avancée d’Office 365 pour la gouvernance, la rétention et l’expiration des données.
* [ ]  Veiller à ce que les politiques antipourriel et de protection d’Exchange Online soient configurées correctement conformément aux [mesures de renforcement des appareils](https://github.com/canada-ca/cloud-guardrails-O365/blob/master/FR/07_Exécuter-le-renforcement-des-appareils.md).
* [ ]  Utiliser Azure Information Protection (AIP) pour la classification, l’étiquetage et la protection des renseignements des documents internes et des courriels pour les points d’extrémité.
 * [ ]  Veiller à ce que les délais d’expiration pour les liens de partage externe soient configurés.

## Autres considérations

* [ ] Partage de documents de contrôle par domaine avec liste blanche ou liste noire
* [ ] Tirer parti d’Office 365 Advanced Data Governance pour la gouvernance, la conservation et l’expiration des données.
* [ ] Utiliser la prévention de la perte de données avec AIP pour assurer une uniformité et une sécurité accrues au-delà de la répartition manuelle des utilisateurs.
* [ ] Configurer les politiques afin d’établir le [cloisonnement de l’information](https://docs.microsoft.com/fr-ca/microsoftteams/information-barriers-in-teams) et empêcher les personnes ou les groupes de communiquer entre eux.
* [ ] Utiliser les [limites de conformité](https://docs.microsoft.com/fr-ca/microsoft-365/compliance/set-up-compliance-boundaries?view=o365-worldwide) afin de créer des limites logiques qui contrôlent l’emplacement du contenu des utilisateurs (comme les boîtes de courriel, les sites SharePoint et les comptes OneDrive) et qui assurent la découverte électronique.

## Validation

* [ ] À déterminer

## Références

1. [AMOPS 2017-01](https://www.canada.ca/en/treasury-board-secretariat/services/access-information-privacy/security-identity-management/direction-secure-use-commercial-cloud-services-spin.html), section 6.2.4.
2. Voir les conseils en matière de cryptographie sous les publications [40.111](https://cyber.gc.ca/fr/orientation/algorithmes-cryptographiques-pour-linformation-non-classifie-protege-et-protege-b) et [40.062](https://www.cse-cst.gc.ca/en/system/files/pdf_documents/itsp.40.062-eng.pdf).
3. Voir les conseils dans [Considérations relatives à l’utilisation de la cryptographie dans les services d’informatique en nuage commerciaux](https://www.canada.ca/fr/gouvernement/systeme/gouvernement-numerique/technologiques-modernes-nouveaux/services-informatique-nuage/consideration-utilisation-de-la-crrptographie-dans-les-services-informatique-en-nauge.html)
4. Voir la section 4.4.1.10 de la [Directive sur les services et le numérique](https://www.tbs-sct.gc.ca/pol/doc-fra.aspx?id=32601)
5. Mesures de sécurité connexes : SC 8, SC 8(1), SC 12, SC 13, SC 17, SC 28, SC 28(1).
