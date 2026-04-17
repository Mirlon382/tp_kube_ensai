# TP7
# remarques
## 2.3
Je vois bien les services qui se lance même sans target_port pour le service. On va quand même le mettre pour ensuite connecter la db.
Je vois pas de pod
## 3.3
J'ai dû recréer le helpers.tpl pour pouvoir upgrade l'appli
Mais ça fonctionne bien :
Events:
  Type    Reason                       Age    From            Message
  ----    ------                       ----   ----            -------
  Normal  CreatingPodDisruptionBudget  3m15s  cloudnative-pg  Creating PodDisruptionBudget ma-release-postgresql-primary
  Normal  CreatingServiceAccount       3m15s  cloudnative-pg  Creating ServiceAccount
  Normal  CreatingRole                 3m15s  cloudnative-pg  Creating Cluster Role
  Normal  CreatingInstance             3m15s  cloudnative-pg  Primary instance (initdb)

## 4.3
Ca me fait penser au docker-compose.override et c'est vraiment pratique