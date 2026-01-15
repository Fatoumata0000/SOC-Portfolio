# Rapport d’incident – Attaque par force brute

## Résumé
Une attaque par force brute a été détectée sur le service SSH du serveur.

## Attaquant
Adresse IP : 185.92.43.17  
Compte ciblé : admin  

## Chronologie
Plusieurs tentatives de connexion échouées ont été observées, suivies d’une connexion réussie.

## Impact
L’attaquant a obtenu un accès au compte administrateur.

## Actions SOC
- Bloquer l’adresse IP
- Réinitialiser le mot de passe du compte admin
- Vérifier les autres connexions
- Analyser les activités après connexion

## Conclusion
Il s’agit d’un incident de sécurité critique.
