# Kristal Wink — architecture de référence proposée

**Date :** 2026-10-12  
**Classe :** C1, orientation architecturale en étude; non dessin d'exécution ni certification.  
**Source d'intention :** `sources/owner-direction/2026-10-12-kristal-wink-offline-kristals-direction.md`.

## Définition

Le **Kristal Wink** est une cellule élémentaire de Kristal Farms : **une éolienne + une charge de calcul IA modulable + une mémoire durable de Kristals + une petite réserve d'énergie pour le fonctionnement minimal/l'arrêt sûr + une interface d'accès local**. Le nœud doit être capable de travailler de façon autonome et intermittente sans fibre haut débit continue lorsque modèles, données, droits et énergie nécessaires sont disponibles localement. Une série de Winks peut ensuite partager des liaisons électriques/numériques et des Kristals; ce maillage est optionnel, non requis au premier déploiement.

## Priorités énergétiques et commande

1. La sûreté électrique, l'intégrité du système et les usages communautaires essentiels sont prioritaires selon un accord d'interface validé. Les périodes de grand froid et autres urgences déclenchent une réduction/hibernation de la charge IA non essentielle.
2. Le calcul est **interruptible** et suit l'excédent réellement utilisable, non la puissance nominale de l'éolienne. En cas de vent réduit, diminuer la production IA; sous seuil, préserver l'état et hiberner.
3. Les contrôleurs et protections matériels, les dispositifs de délestage et les procédures d'urgence doivent fonctionner indépendamment de l'orchestrateur IA.
4. Sauvegarder les tâches par points de contrôle idempotents : l'arrêt ne doit pas corrompre un Kristal; au retour de l'énergie, vérifier puis reprendre.
5. Ne jamais inférer qu'un réseau villageois dispose de MW de surplus; tout raccordement, îlotage, transfert ou priorisation réelle demande études et autorisations.

États de travail conceptuels : `PRODUIRE`, `REDUIRE`, `HIBERNER`, `SECURISER`. Les seuils, réserves et marges de sécurité doivent être définis par études électriques et accords communautaires, pas par une IA générative.

## Batteries et autonomie réelle

Une réserve **modeste** peut alimenter contrôle, stockage, télécom minimum, mise en sécurité et arrêt ordonné; le traitement lourd ne doit pas dépendre d'un vaste stockage pour rester en fonctionnement sans vent. Cette minimisation vise coûts, matériaux et impacts, sans préjuger de l'analyse de cycle de vie ni du besoin réel de réserve. Une éolienne unique ne constitue **pas** une garantie d'approvisionnement continu d'un village, ni un système de secours autonome certifié.

## Intégration physique

Implanter l'IA, le stockage et certaines batteries **dans la tour** est une option de conception, sous réserve de la sécurité incendie, des exigences fabricant, vibrations, températures, humidité, accès de maintenance, résistance aux intempéries, comptage et conformité électrique. La solution alternative préférentielle à évaluer est un local technique au pied de la tour ou adjacent. La disponibilité éolienne en conditions de givre/tempêtes est à mesurer.

## Réseau et transport de valeur

Le Wink produit des Kristals transportables sans exiger une liaison fibre à haut débit 24/7 pour les tâches différables. Synchronisation opportuniste, support physique chiffré, bateau/avion ou sous-ensembles vérifiables sont des possibilités. Une connexion minimale peut rester nécessaire pour certaines fonctions de maintenance, sécurité, licences, mises à jour et communications; chaque charge doit documenter ses dépendances. Les services de location connectée nécessitant latence/débit continus continuent d'employer la fibre si le profil de service l'impose.

## Gouvernance

Le principe proposé associe règles communes fixées selon une procédure par l'Assemblée des fondateurs, gouvernance locale effective et garanties anti-capture. Aucun pouvoir central ne supprime les droits, le consentement ni les mécanismes de recours des communautés concernées. Voir `docs/00-control/KRISTAL_GOUVERNANCE_COLLECTIVE_FR.md`.

## Conditions de preuve d'un pilote Wink

- Courbes éoliennes réelles, variabilité saisonnière, givrage/arrêts et énergie nette disponible pour calcul après charges prioritaires.
- Puissance minimum, régime de pause/reprise, efficacité énergétique totale, stabilité du stockage et contrôles indépendants.
- Risques et coût du site (fondation, tour ou local adjacent, maintenance, assurances, incendie, logistique, réglementation).
- Performance/qualité des Kristals produits hors ligne, mécanismes de livraison et vérification d'intégrité.
- Coût complet par unité utile vendue, délai de vente, contrats/demande réelle et conditions d'une rentabilité **avant fibre**.
- Droit, processus de consultation et accords d'interface électrique/sociale avec la communauté.

Le Wink est une **hypothèse de nœud autonome de calcul et de connaissance**, pas la promesse d'un village autosuffisant ni un site approuvé.
