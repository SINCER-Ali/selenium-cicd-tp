1. Avantages observés

Automatisation des tests : Ça nous a permis de vérifier rapidement que toutes les fonctionnalités de la calculatrice fonctionnent, sans refaire les tests manuellement à chaque modification.

CI/CD : Il assure que chaque modification sur develop ou main est automatiquement testée, ce qui réduit les erreurs et améliore la qualité du code.

2. Défis rencontrés

Selenium : La configuration du driver Chrome et la gestion des chemins pour ouvrir la page locale ont été un peu délicates.

Améliorer la stabilité : On peut utiliser des wait explicites pour s’assurer que les éléments sont chargés avant d’interagir avec eux, et faire tourner les tests en environnement identique à la production (headless CI).

3. Métriques

Importantes :

Nombre de tests passés/échoués

Temps de chargement de la page

Couverture du code (pytest-cov)

Efficacité du CI/CD : On peut la mesurer en regardant si tous les tests passent automatiquement après chaque push, et combien de temps le pipeline prend pour détecter les erreurs.