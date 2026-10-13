# Architecture de référence du projet Kristal Farms

## Thèse centrale

Kristal Farms est une architecture d’accès aux ressources énergétiques nordiques. L’inversion centrale est :

> **amener une charge de calcul flexible à l’énergie éloignée, protéger les besoins communautaires et exporter la valeur en Kristals transportables ou par fibre pour les services connectés, plutôt que dépendre par défaut de longs corridors électriques.**

La réduction ou l’évitement des longues routes et lignes HV est une proposition de valeur structurelle primaire. Elle n’est pas présumée universellement avantageuse : l’économie doit être démontrée corridor par corridor et site par site.

## Géographie

- Côte-Nord : géographie de pilote/apprentissage.
- Québec nordique et Labrador : territoire de déploiement à long terme où l’éloignement des routes/HV peut créer le contraste structurel le plus fort.

## Architecture physique

Trois dispositions restent valides : calcul près de la centrale, calcul près du village/port, ou architecture hybride. Le choix dépend de la distance électrique, de la valeur de la chaleur, de la fibre, de la logistique, de l’environnement, de la maintenance, de la sécurité et du choix communautaire.

## Modèle commercial du calcul

Kristal Farms peut offrir des sites/pads de calcul viabilisés plutôt que posséder tous les serveurs. L’infrastructure commune peut fournir alimentation électrique, interface de refroidissement, fibre, sécurité, comptage/télémétrie et accès logistique. Les locataires gardent la souveraineté sur leur matériel, OS, modèles, données, clés et télémétrie interne.

## Priorité énergétique communautaire

Les réseaux villageois existants sont une infrastructure communautaire protégée; ils ne sont pas présumés fournir plusieurs MW disponibles au calcul. L’architecture étudiée est principalement :

> **nouvelle production → priorité communautaire protégée → calcul interruptible → Kristals portables / services connectés par fibre selon besoin**

Les charges communautaires/critiques ont priorité sur le calcul interruptible.

## Chaleur

La chaleur est un coproduit utile, pas une règle universelle de localisation. Elle est récupérée lorsque sa valeur utile dépasse le coût et la complexité de récupération/distribution.

## Réseau et modularité

Le programme peut utiliser des projets hydro/renouvelables petits, moyens ou plus grands lorsque justifiés, avec une croissance du calcul pad par pad. Des nœuds réussis peuvent former un chapelet côtier/de bassins relié principalement par fibre et logistique maritime, avec des interconnexions électriques plus courtes lorsqu’elles apportent de la résilience.

## Gouvernance internationale des locataires

Kristal Farms vise un marché international tout en restant sélectif sur ses contreparties. L'admissibilité est établie avant l'accès à partir de la juridiction, de la propriété effective et du contrôle, des sanctions/contrôles commerciaux et d'une diligence raisonnable de conduite responsable. La politique actuelle du propriétaire exclut les contreparties établies ou contrôlées aux États-Unis des rôles de locataire, acheteur ferme principal (*anchor offtaker*) et opérateur-locataire.

Cette exclusion commerciale ne constitue pas, à elle seule, un embargo sur l'origine technologique.

## Location aveugle au contenu

L'environnement normal est un **environnement chiffré sous contrôle du locataire** (raccourci commercial : location « black box »). Kristal Farms exploite le plan des services physiques partagés; le locataire contrôle le calcul privé. L'exploitation normale n'exige pas l'accès de Kristal Farms aux modèles privés, jeux de données, contenus applicatifs ou clés cryptographiques du locataire.

La conformité repose donc sur la contrepartie et le contrat plutôt que sur l'inspection du contenu. Voir `docs/00-control/INTERNATIONAL_TENANT_GOVERNANCE.md` et `docs/security/TENANT_CONFIDENTIALITY_BOUNDARY.md`.

## Gouvernance et anti-capture

Le capital peut financer l’infrastructure sans acquérir automatiquement le contrôle de la terre, du logement, de l’énergie, du port, de la fibre, de l’emploi et de la gouvernance communautaire.

## État du screening

Il n’existe **aucun classement actif de sites**. Toute priorisation future exige des preuves transparentes en hydrologie, terrain/head, environnement, gouvernance communautaire/autochtone, logistique, télécom, architecture électrique et économie actuelle.

## Profil Kristal Wink et transport hors ligne (orientation du 12 octobre 2026)

Une **cellule de départ** peut être une seule éolienne avec calcul IA dont la puissance suit le vent, stockage local durable des Kristals, petite réserve d'arrêt sûr et accès local. En cas de baisse du vent ou de demande prioritaire du village (notamment grands froids), le calcul est réduit ou hiberné sans interrompre les protections indépendantes du système électrique. L'équipement dans la tour n'est qu'une option soumise à vérifications fabricant, incendie, thermique, entretien et conformité. Voir [architecture Wink](KRISTAL_WINK_ARCHITECTURE_FR.md).

Les [Kristals transportables et opératoires](KRISTALS_OFFLINE_ET_PROCEDURES_FR.md) ouvrent une voie hors ligne : la valeur peut être livrée ultérieurement par lien opportuniste ou support physique chiffré. Cela n'annule pas les exigences de fibre des locataires connectés. La rentabilité avant fibre reste à démontrer; le modèle de frontière économique historique concernait l'export connecté, non ce nouveau profil.

La [gouvernance collective](../00-control/KRISTAL_GOUVERNANCE_COLLECTIVE_FR.md) est proposée autour de paramètres communs établis par une Assemblée des fondateurs et de pouvoirs locaux effectifs, sous réserve du droit et du consentement des communautés. Une seule éolienne ne garantit pas l'énergie ferme du village.
