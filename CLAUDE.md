# CLAUDE.md

Dépôt public : ne jamais y écrire de données privées (noms de tiers, banques, montants, clients, identifiants).

## Projet

Logiciel de planning Gantt de chantier avec estimatif de coûts, pour la construction et la rénovation.
Utilisateur cible : une entreprise BTP tous corps d'état (rénovation, démolition, construction, gestion de projet) qui travaille en direct et en sous-traitance, en France (Alsace), Allemagne et Suisse.

État : dépôt vide, aucune stack choisie. Avant d'écrire du code, proposer une stack avec une recommandation tranchée et la faire valider.

## Règles métier que le logiciel doit respecter

Planning
- Chaque tâche a une durée de base et une marge d'aléas séparée, réglable, 15 à 25 % par défaut. La marge reste visible, jamais fondue dans la durée.
- Les approvisionnements sont des tâches à part entière, placées avant la pose : commande, fabrication, livraison. Commandes spéciales (parquet, menuiseries sur mesure, carrelage importé) : 4 à 12 semaines.
- Les validations administratives bloquent le démarrage : déclaration préalable 1 mois, permis de construire 2 à 3 mois minimum.
- Calendriers distincts par pays (jours fériés FR, DE, CH, y compris les fériés propres à l'Alsace-Moselle et aux cantons), plus les congés CIBTP.
- Les tâches extérieures portent un indicateur de sensibilité météo.
- Un retard sur une commande spéciale doit faire apparaître son effet sur la date de fin.
- La date annoncée au client est la date avec aléas, jamais la date au plus tôt.

Estimatif
- Coût par tâche : main-d'œuvre, matériaux, sous-traitance, location de matériel.
- Totaux HT, TVA et TTC, avec taux de TVA réglable par ligne et par pays.
- Devise par chantier : EUR ou CHF.
- Affichage du prix de revient, du prix de vente et de la marge.

## Façon de travailler

- Répondre en français, termes techniques en anglais acceptés.
- Direct et factuel. Recommandation tranchée, pas de « ça dépend ». Si une idée est mauvaise ou risquée, le dire avec les raisons.
- Sur un sujet critique, donner un plan A et un plan B.
- Tâches opérationnelles en checklist à cases (☐), comparaisons et jalons en tableau, raisonnement en prose.
- Tout délai donné est une fourchette, avec ce qui la conditionne.
- Lister les risques avant toute communication à un client.
- Interface, libellés et documentation en français.
