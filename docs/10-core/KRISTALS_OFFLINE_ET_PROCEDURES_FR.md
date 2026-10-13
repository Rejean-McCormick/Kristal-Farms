# Kristals hors ligne, transportables et opératoires

**Date :** 2026-10-12  
**Classe :** C1, direction de produit/architecture à valider; ce document ne crée pas de contrat d'interopérabilité v10 ni de fonctionnalités déjà livrées.

## Nouvelle voie de création de valeur

Deux produits peuvent coexister :

- **Kristals cristallisés hors ligne** : tâches de calcul différables, connaissances, raisonnements structurés, relations, hypothèses et résultats conservés dans des unités logiques portables. Livraison numérique lorsque possible ou transport physique chiffré (avion/bateau), éventuellement par parties.
- **Calcul connecté/serviced pads** : charges de travail requérant fibre continue, latence, volumes transférés ou niveau de service élevé, avec responsabilités d'hébergement et confidentialité des locataires inchangées.

Le besoin de fibre doit être un **paramètre de chaque charge**, et non une condition universelle pour démarrer une cellule Wink. Le transport physique a des délais et coûts; il ne remplace pas tous les flux interactifs.

## Kristal comme état de pensée explicite

L'IA peut produire des Kristals plutôt que laisser son travail se perdre dans un chat ou un document opaque. Chaque Kristal devrait déclarer : identité logique, version, domaine, provenance, axes/orientations d'exploration, statut épistémique, incertitudes, dépendances, intégrité, autorisations et modes de consultation.

Les Kristals peuvent évoluer du contenu structuré vers les **Kristals opératoires** : une procédure stabilisée, limitée, validée et réexécutable sur un appareil local pour réduire les coûts de raisonnement. Une telle compilation n'est jamais un raccourci autour de la validation; un processus doit déclarer ses préconditions, critères de sortie, autorité, garde-fous, test de non-régression, budget de calcul/énergie, et déclencheurs d'escalade vers un orchestrateur plus général.

La stabilité d'une procédure ne garantit pas qu'elle généralise à un nouveau contexte. L'utilisateur et l'orchestrateur doivent pouvoir remettre en question, corriger ou arrêter les résultats.

## Interfaces humaines

Les points d'entrée envisagés : **texte, voix adaptée à la langue et à l'accent de la personne, photographie, son**. Une couche locale interprète ces signaux en intentions *probables* puis propose les orientations et Kristals pertinents. Le traitement en périphérie dépend du matériel et des modèles disponibles; les performances doivent être mesurées.

Le ton vocal peut fournir des indices contextuels incertains sur un **état émotionnel momentané**, jamais un accès certain aux émotions. Ce module doit être opt-in, local, effaçable, explicable, corrigeable et désactivé par défaut, sans profil émotionnel durable, publicité ciblée ni inférence médicale. Aucun service essentiel ne peut être conditionné à ce profil.

## Contrat de transport proposé (à spécifier et tester)

Le paquet ou fragment devrait comporter : ID logique, version, manifeste des fragments, sommes de contrôle et signature/authenticité, dépendances, provenance, niveau de confidentialité, chiffrement, politique d'accès, limites d'utilisation et protocole de restauration/synchronisation. Une réception partielle ne doit jamais se déclarer complète. Rotation/perte de clés, révocation, incompatibilités de versions, sauvegarde et conflits doivent être gérés.

Éviter tout conflit de vocabulaire avec les contrats formels de Kristal v10. Ce texte est une **exigence de conception future**, pas une affirmation que le protocole et la compatibilité sont déjà spécifiés.

## Mesures de viabilité

Évaluer par charge le coût énergie/production/reprise, la qualité et la stabilité, la taille et le coût de livraison, la fréquence des mises à jour, la valeur pour un acheteur vérifié, l'accès hors ligne et le bénéfice réel pour la communauté. La rentabilité avant fibre demeure une hypothèse à vérifier.
