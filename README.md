# Exercices Kubernetes

Mettre en place les ressources demandées à chaque niveau.

```
✅ : Correction présente
❌ : Correction à faire
🚧 : Correction en cours
```

## ✅ Niveau 1:
- 1 pod de base de données
- 1 service devant cette base
- 1 pod web permettant de requêter la base de donnée (adminer par exemple)
- 1 service devant le pod web

## ✅ Niveau 2:
- 1 volume pour le stockage des données de la BDD (et reconfiguration du pod)
- 1 volume pour les données du serveur web (et reconfiguration du pod)

## ✅ Niveau 3:
- 1 configmap pour la config de la base de donnée
- 1 secret pour le mot de passe admin de la base de données

## ✅ Niveau 4:
- Passer les pods en déploiement
- 3 pods web permettant de requêtes la base de donnée avec une ancienne version de adminer
- Suppression d’un pods (quel est le comportement de k8s ?)

## ✅ Niveau 5:
- Création d’un Helm chart pour permettre de déployer plus simplement et plus rapidement
- Déploiement d’une seconde infra identique dans un second namespace

## 🚧 Niveau 6:
- Déploiement chez OVH
- 1 ingress pour permettre d’accéder à notre infra depuis internet

## ❌ Niveau 7:
- Supervision de base avec Grafana / Prometheus

---
### Ressources
- [Helm](/helm) : Templates et values pour démarrer quelques services via Helm