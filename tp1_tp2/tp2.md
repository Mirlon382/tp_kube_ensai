On va écrire un deployment.yaml pour aller chercher une image sur dockerhub (image_dockerhub.png). Mon image semble ne pas fonctionner donc je vais utiliser celle d'Emile et lancer le deployment.

Parmi les screens, on trouve :

logs_pre_test.png Les 3 images se sont bien déployés.

curl_app.png on va rentrer dans le container et exécuter curl sur le localhost

logs_post_test.png On voit bien le log de 2 requetes GET effectuée par le curl sur une des images. 

describe_deployment.png on va describe la stack de deployment

describe_pod.png on va describe le pod, son historique par exemple

get_deploy.png on voit 3 stacks. Les stacks containers* ont échoué à cause de mon image. La stack api server se déploie bien.

list_dep.png On va lister les dépendances Python associées en rentrant dans le container puis pip list

