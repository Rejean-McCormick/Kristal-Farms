# ADR-0024 — Profil Kristal Wink offline-first, calcul interruptible et export portable

**Statut : proposé (orientation 2026-10-12; implémentation non adoptée)**

## Contexte

L'architecture initiale privilégie un corridor fibre de grande capacité pour exporter la valeur d'une charge numérique. L'orientation récente ajoute une classe de charges différables : l'IA transforme du calcul local en Kristals transférables plus tard par liaison opportuniste ou support physique. Une cellule d'une seule éolienne (« Kristal Wink ») peut ainsi, sous conditions, produire localement même sans fibre permanente.

## Décision architecturale proposée

- Traiter la fibre comme une **dépendance par profil de charge**, indispensable à certaines offres connectées mais non universelle pour la cristallisation différable.
- Garantir la **priorité communautaire** par contrôle électrique/sûreté indépendant; rendre le calcul interruptible, avec hibernation, checkpoints et reprise contrôlée selon vent et température/besoins prioritaires.
- Évaluer une éolienne + calcul/stockage local + réserve minimale comme cellule pilote; liaison à d'autres cellules optionnelle.
- Exiger identité, provenance, intégrité, confidentialité, accès et gestion de fragments pour le transport de Kristals; ne pas prétendre qu'une nouvelle norme Kristal est déjà opérationnelle.
- Encadrer les décisions par une gouvernance collective anti-capture, selon charte à formaliser et sans remplacer les droits locaux/consentements.

## Non-décisions

Aucun site, turbine, puissance, batterie, emplacement dans la tour, budget, rentabilité avant fibre, norme d'interopérabilité Kristal opératoire ni structure juridique ne sont ici approuvés. Les services connectés et les engagements des locataires existants ne sont pas supprimés.

## Compatibilité et suite

L'ADR explicite une nouvelle option; il ne remplace ni les ADR de confidentialité, ni les contrats de données/observations/scénarios. Faire suivre d'études électriques, prototype de reprise, modèle économique par type de charge, schéma de gouvernance validé, exigences de sécurité et tests d'intégrité/portabilité.

Voir `docs/10-core/KRISTAL_WINK_ARCHITECTURE_FR.md`, `docs/10-core/KRISTALS_OFFLINE_ET_PROCEDURES_FR.md`, `docs/00-control/KRISTAL_GOUVERNANCE_COLLECTIVE_FR.md`.
