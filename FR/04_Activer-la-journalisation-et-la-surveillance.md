# Activer la journalisation et la surveillance

([Retourner](/README.md#mesures-de-sécurité-initiales))

## Objectif

Continuellement surveiller les événements et la performance du système et inclure une fonction de dossiers d’audit en matière de sécurité dans tous les systèmes d’information afin de permettre la détection des incidents. Il est essentiel d’avoir un niveau adéquat de journalisation et de surveillance, y compris une fonction de dossiers d’audit en matière de sécurité dans tous les systèmes d’information hébergés dans l’environnement de nuage et pour les charges de travail en nuage.

## Principales considérations

### Journalisation

* Veiller à ce que l’audit de la boîte de courriels pour tous les utilisateurs soit activé.
* Veiller à ce que la recherche du journal d’audit Microsoft 365 soit activée.
* Tirer profit de l’[API Activité de gestion Office 365](https://docs.microsoft.com/fr-ca/office/office-365-management-api/office-365-management-activity-api-reference) pour récupérer les renseignements concernant les actions et les événements d’utilisateur, d’administrateur, de système et de politique des journaux d’activités d’Office 365 et d’Azure AD.
* Indiquer les événements dans la solution qui doivent être audités conformément à la [Journalisation des événements du GC](https://www.gcpedia.gc.ca/gcwiki/images/e/e3/GC_Event_Logging_Strategy.pdf).
* Configurer le service pour envoyer les journaux d’audit à une installation centralisée de journalisation, si disponible.

### Surveillance

* Surveiller continuellement les événements et la performance des systèmes. Veiller à ce que les rapports soient examinés au moins chaque semaine, notamment :
  * rapports sur l’accès pour tous les comptes d’administrateur;
  * rapport « Connexions à risque » d’Azure AD;
  * changements de groupe du rôle d’utilisateur;
  * rapport d’activité d’approvisionnement de compte;
  * affectations au groupe du rôle d’administrateur non général;
  * rapport d’activité de réinitialisation des mots de passe libre-service;
  * rapport sur les correspondances de stratégie de protection contre la perte de données (DLP);
  * rapport d’incidents DLP;
  * rapports de remplacements et faux positifs DLP.
* Configurer les alertes et les notifications à envoyer à la personne-ressource ou à l’équipe appropriée de l’organisation.
* Configurer ou utiliser une source de temps faisant autorité aux fins d’estampille temporelle des documents d’audit produits par les composants de votre solution.
* Élaborer un plan pour répondre aux répercussions des incidents de sécurité, et les comprendre, conformément au [Plan de gestion des événements de cybersécurité du GC](https://www.canada.ca/fr/secretariat-conseil-tresor/services/acces-information-protection-reseignements-personnels/gestion-securite-identite/plan-gestion-evenements-cybersecurite-gouvernement-canada.html).
* Établir un protocole d’entente (PE) pour les services de défense et de surveillance des menaces avec le Centre canadien pour la cybersécurité (CCC).

## Autres considérations

* L’utilisation d’une solution de journalisation centralisée devrait être considérée dans la mesure du possible. Les capacités qui automatisent l’analyse des événements et des comportements et offrent des alertes en temps réel peuvent aider à cerner les menaces et les incidents de sécurité possibles.

## Validation

* Confirmer que la stratégie de journalisation des événements est mise en œuvre.
* Confirmer la production des journaux d’événements.
* Confirmer que les coordonnées de sécurité ont été configurées pour recevoir des alertes et des notifications.
* Confirmer qu’un plan est en place pour répondre aux incidents.

## Références

1. [Directive sur la gestion de la sécurité, annexe B : Procédures obligatoires relatives aux mesures de sécurité de la technologie de l’information](https://www.tbs-sct.canada.ca/pol/doc-fra.aspx?id=32611), sous-section B.2.3.2.8.
2. [AMOPS 2017-01](https://www.canada.ca/en/treasury-board-secretariat/services/access-information-privacy/security-identity-management/direction-secure-use-commercial-cloud-services-spin.html), sections 6.3 et 6.3.1.
3. Les 10 principales mesures de sécurité du CST, numéro 1, 5 et 8.
4. Voir l’[Orientation sur la journalisation des événements du GC](https://www.gcpedia.gc.ca/gcwiki/images/e/e3/GC_Event_Logging_Strategy.pdf)
5. Mesures de sécurité connexes : AU-2, AU-3, AU-6, AU-8, AU-9, AU-9(4), AU-12, SI-2, SI-4.
