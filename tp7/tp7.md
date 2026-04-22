# TP7
# remarques
## 2.3
Les services se lancent même sans target_port. On va quand même le mettre pour ensuite connecter la db.

## 3.3
J'ai dû recréer le helpers.tpl pour pouvoir upgrade l'appli
Mais ça fonctionne bien, en preuve ce log 
Events:
  Type    Reason                       Age    From            Message
  ----    ------                       ----   ----            -------
  Normal  CreatingPodDisruptionBudget  3m15s  cloudnative-pg  Creating PodDisruptionBudget ma-release-postgresql-primary
  Normal  CreatingServiceAccount       3m15s  cloudnative-pg  Creating ServiceAccount
  Normal  CreatingRole                 3m15s  cloudnative-pg  Creating Cluster Role
  Normal  CreatingInstance             3m15s  cloudnative-pg  Primary instance (initdb)

## 4.3
Ca me fait penser au docker-compose.override. C'est vraiment pratique
