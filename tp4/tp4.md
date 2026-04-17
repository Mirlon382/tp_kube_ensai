# TP4

Application du cours sans soucis jusqu'à 1/la configmap 2/l'ajout du statefulset. 
1/la configmap est spécifique à l'image du backend, ce qui avait tendance à faire crash le backend jusqu'à ce que j'applique les bons noms de variable
2/J'ai dû comprendre que mon pvc n'était pas dans le bon format. Après avoir relancé mon deployement, ça a fonctionné.