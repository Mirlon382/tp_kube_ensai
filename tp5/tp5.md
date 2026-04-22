# tp5
On crée une image v1 avec l'endpoint /health exposé sur le port 8000 et une image v2 avec l'endpoint /ensai.
On utilise des probes sur l'endpoint /health. Le pod est en état "running" à partir de 10s

## rolling update
Quand on applique le api_rolling.yaml, ça lance le processus de rolling update. La commande rollout va permettre de suivre le processus.
Il n'y a pas eu de difficultés.
