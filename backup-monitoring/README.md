# Monitoring Helm Chart

Ce chart Helm déploie une stack de monitoring complète avec Prometheus et Grafana pour surveiller un cluster Kubernetes et l'application `sockshop`. Voici tout ce qu'il faut savoir pour l'utiliser, avec les alertes et dashboards configurés.

## Prérequis

- Un cluster Kubernetes opérationnel (testé sur v1.28).
- Helm 3 installé (`helm version` pour vérifier).
- L'application `sockshop` déployée dans un namespace (par exemple, `sockshop-namespace`).
- Un canal Slack pour les notifications (voir la section Alertmanager).

## Déploiement

1. Clone le repo et va dans le dossier `monitoring` :
   ```bash
   cd helm-charts/monitoring

   