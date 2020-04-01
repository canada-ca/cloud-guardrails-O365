# Exécuter le renforcement des appareils

## Objectif

La position de sécurité des appareils utilisés pour avoir accès au service devrait être considérée. À tout le moins, les organisations doivent veiller à ce que les appareils aient les plus récentes mises à jour installées, n’utilisent pas les privilèges d’administrateur, aient des mesures de protection contre les logiciels malveillants et collectent des journaux de sécurité.

## Principales considérations

* [ ] Empêcher tout appareil non autorisé à avoir accès à des renseignements opérationnels ou personnels de nature sensible.
* [ ] Utiliser les points d’extrémité gérés par le GC et confirmer que l’appareil est conforme, comme exiger une version minimale et prise en charge du système d’exploitation.
* [ ] Conformément à [l’AMPTI 2018-03](https://www.canada.ca/fr/gouvernement/systeme/gouvernement-numerique/technologiques-modernes-nouveaux/avis-mise-oeuvre-politique/directive-migration-configuration-systeme-exploitation-bureau-windows10.html), pour les appareils Windows 10, la version minimum du GC de Windows 10 et la configuration indiquées dans la page sur les [niveaux de référence pour la configuration de Windows 10 du GC](https://gcconnex.gc.ca/groups/profile/12903340/wtd-common-desktop-operating-environment-environnement-dexploitation-commun-des-ordinateurs-de-bureau-des-atmt?language=en#20998653) (accessible seulement sur le réseau du gouvernement du Canada) doivent être mises en œuvre. La norme de configuration minimale du GC prescrit des normes de configuration de Windows 10 qui sont nécessaires pour maintenir la sécurité des réseaux et des appareils technologiques en milieu de travail du GC.


### Mobile Device Management

* [ ] Ensure mobile device management polices are set to require advanced security configurations to protect from basic internet attacks
* [ ] Ensure mobile devices require the use of a password
* [ ] Configure mobile device password policy is configured, in accordance with [GC Password Guidance](https://www.canada.ca/en/government/system/digital-government/password-guidance.html).
* [ ] Ensure that users cannot connect from devices that are jail broken or rooted
* [ ] Configure settings to lock multiple devices after a period of inactivity to prevent unauthorized access
* [ ] Ensure that mobile device encryption is enabled to prevent unauthorized access to mobile data
* [ ] Ensure that devices connecting have AV and a local firewall enabled
* [ ] Ensure mobile device management policies are required for email profiles

## Validation

* [ ] TBD

## References

1. [SPIN 2017-01](https://www.canada.ca/en/treasury-board-secretariat/services/access-information-privacy/security-identity-management/direction-secure-use-commercial-cloud-services-spin.html)
2. CSE Top 10
3. Refer to [CCCS ITSP.30.031 V2 User Authentication Guidance for Information Technology Systems](https://cyber.gc.ca/en/guidance/user-authentication-guidance-information-technology-systems-itsp30031-v3)
4. Refer to the [GC Password Guidance](https://www.canada.ca/en/government/system/digital-government/password-guidance.html)
5. Refer to the [ITPIN 2018-03](https://www.canada.ca/en/government/system/digital-government/modern-emerging-technologies/policy-implementation-notices/direction-windows10-desktop-operating-system-migration-configuration.html)
