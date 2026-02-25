# Prototype NFC + Authentification biométrique

## Installation
1. Cloner le dépôt : `git clone <url>`
2. Installer les dépendances : `pip install -r requirements.txt`
3. Configurer l’environnement : Python 3.10+, OpenCV, PyNFC

## Exécution
- Lancer une transaction simulée : `python src/run_transaction.py --mode fingerprint`
- Simuler une attaque spoofing : `python experiments/spoof_attack.py --dataset data/fingerprint`
- Générer les logs : résultats dans `results/logs/`

## Sorties attendues
- Taux de faux positifs/négatifs
- Temps de réponse
- Journalisation des attaques réussies/échouées

## Reproductibilité
- Seeds fixés dans `config/seeds.json`
- Splits de données définis dans `config/splits.json`
- Paramètres expérimentaux documentés dans `experiments/config.yaml`
