# Mettre en œuvre la protection des données

([Retourner](README.md#mesures-de-sécurité-initiales))

## Objectif

Protéger les renseignements et les actifs hébergés dans le nuage de l’accès, de l’utilisation, de la divulgation, de la modification, de l’élimination, de la transmission ou de la destruction non autorisés tout au long de leur cycle de vie.

## Principales considérations

* Demander des conseils aux responsables de la protection des renseignements personnels et de l’accès à l’information dans les institutions avant de stocker des renseignements personnels dans les environnements d’informatique en nuage.
* Vérifier l’emplacement du service, conformément à la section 4.4.1.10 de la [Directive sur les services et le numérique](https://www.tbs-sct.canada.ca/pol/doc-fra.aspx?id=32601).
* Veiller à ce que les données en transit soient chiffrées par défaut (p. ex., TLS v1.2).
* Appliquer les mécanismes de chiffrement pour protéger la confidentialité et l’intégrité des données hébergées dans le service d’informatique en nuage.
* Utiliser les algorithmes et les protocoles cryptographiques approuvés par le Centre de la sécurité des télécommunications Canada (CSTC), conformément aux publications [40.111](https://cyber.gc.ca/fr/orientation/algorithmes-cryptographiques-pour-linformation-non-classifie-protege-et-protege-b) et [40.062](https://www.cse-cst.gc.ca/fr/system/files/pdf_documents/itsp.40.062-fra.pdf).
* Activer les politiques de prévention de la perte de données (DPL) au niveau du service d’informatique en nuage afin de permettre au contenu sur Exchange Online et SharePoint Online d’être analysé pour des types particuliers de données comme les numéros de sécurité sociale, les numéros de carte de crédit ou les mots de passe.
* Configurer les stratégies de classification des données pour protéger les documents et les courriels internes.
* Veiller à ce que les délais d’expiration pour les liens de partage externe soient configurés.
* Veiller à ce que les utilisateurs externes ne puissent pas partager des fichiers, des dossiers et des sites qu’ils ne possèdent pas.
* Veiller à ce que le partage de fichiers externes dans les équipes soit activé uniquement pour les services de stockage approuvés dans le nuage.

## Autres considérations

* Contrôle du partage de documents par domaine avec liste verte ou liste d’exclusion.
* Explorer la Gouvernance des données avancée d’Office 365 pour la gouvernance, la rétention et l’expiration des données (licence supplémentaire requise).
* Explorer l’utilisation de DLP automatisé avec Azure Information Protection pour davantage de cohérence et de sécurité au-delà de l’affectation manuelle des utilisateurs (licence supplémentaire requise).
* Enquêter sur l’établissement de politiques comportant des [barrières à l’information (IB)](https://docs.microsoft.com/fr-ca/microsoftteams/information-barriers-in-teams) afin d’empêcher des personnes ou des groupes de communiquer entre eux (autorisation supplémentaire requise).
* Enquêter sur l’utilisation des [limites de conformité](https://docs.microsoft.com/fr-ca/microsoft-365/compliance/set-up-compliance-boundaries?view=o365-worldwide) afin de créer des limites logiques qui contrôlent l’emplacement du contenu des utilisateurs (comme les boîtes de courriel, les sites SharePoint et les comptes OneDrive) et qui appuient eDiscovery.

## Validation

* À déterminer

## Références

1. [Directive sur la gestion de la sécurité, annexe B : Procédures obligatoires relatives aux mesures de sécurité de la technologie de l’information](https://www.tbs-sct.canada.ca/pol/doc-fra.aspx?id=32611), sous-section B.2.3.4.
2. [AMOPS 2017-01](https://www.canada.ca/en/treasury-board-secretariat/services/access-information-privacy/security-identity-management/direction-secure-use-commercial-cloud-services-spin.html), section 6.2.4.
3. Voir les conseils en matière de cryptographie sous les publications [40.111](https://cyber.gc.ca/fr/orientation/algorithmes-cryptographiques-pour-linformation-non-classifie-protege-et-protege-b) et [40.062](https://www.cse-cst.gc.ca/en/system/files/pdf_documents/itsp.40.062-eng.pdf).
4. Voir les conseils dans [Considérations relatives à l’utilisation de la cryptographie dans les services d’informatique en nuage commerciaux](https://www.canada.ca/fr/gouvernement/systeme/gouvernement-numerique/technologiques-modernes-nouveaux/services-informatique-nuage/consideration-utilisation-de-la-crrptographie-dans-les-services-informatique-en-nauge.html)
5. Voir la section 4.4.1.10 de la [Directive sur les services et le numérique](https://www.tbs-sct.gc.ca/pol/doc-fra.aspx?id=32601)
6. Mesures de sécurité connexes : SC 8, SC 8(1), SC 12, SC 13, SC 17, SC 28, SC 28(1).
