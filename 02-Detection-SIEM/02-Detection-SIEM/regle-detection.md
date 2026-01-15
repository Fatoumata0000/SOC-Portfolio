# Règle de détection – Attaque par force brute

## Nom
Détection Brute Force SSH

## Logique
Déclencher une alerte lorsqu’une même adresse IP génère 4 échecs de connexion ou plus
sur un même compte dans un court intervalle de temps.

## Pseudo-règle SIEM (Splunk / ELK)

Si:
- event.action = "failed login"
- et même IP source
- et même utilisateur
- et nombre d’événements ≥ 4 en moins de 2 minutes

Alors:
- Générer une alerte SOC
- Priorité: Élevée
