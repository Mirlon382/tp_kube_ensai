## Note TP1

### Ex1
Ok pour la phase de build du container et le start (bien penser à lier un port du container à un port de la machine). Pour pousser l'image : login->tag->push

Difficultés :
FastAPI a besoin d'uvicorn pour servir ses endpoints. Pour cela, on ajoute dans le layer CMD uvicorn, une ip et un port associé. Je suis habitué à mettre directement dans le code un bloc type : if name == main : uvicorn run ...
Pour s'en rendre compte, il est facile d'ouvrir un terminal bash dans le container avec le flag -it après on va pouvoir lister les process en cours

Note :
Importance d'utiliser les images slim et les images distroless pour la sécurité et le poids final du container
Comment gérer les secrets? On va ajouter un layer ENV (ex. ENV WORD="ENSAI").
Pour éviter de bloquer un terminal, il faut ajouter le flag -d

### Ex2

Pour le multistage build, on va suivre les instructions du cours avec java21 au lieu de 17. Le container se build avec l'application java sans problèmes.

Note :
whitelabel error page sur root (voir code)
ok pour l'endpoint /hello
possible d'attacher un volume

-> C'est sensiblement la même chose que la correction