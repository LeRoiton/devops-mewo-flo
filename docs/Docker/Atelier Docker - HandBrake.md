# Atelier Docker - HandBrake

## Quelle commande utiliseriez-vous pour télécharger l'image Docker de HandBrake?
```bash
docker pull jlesage/handbrake
```
## Comment lanceriez-vous un conteneur HandBrake pour traiter une vidéo située sur votre machine hôte?
```bash
docker run -d --name=handbrake -p 5800:5800 -v /docker/appdata/handbrake:/config:rw -v /home/user:/storage:ro -v /home/user/HandBrake/watch:/watch:rw -v /home/user/HandBrake/output:/output:rw jlesage/handbrake
```
## Quelles commandes permettent d'inspecter les détails et les logs d'un conteneur actif?
```bash
docker inspect f3bb8db84b52
```
```bash
docker logs f3bb8db84b52
```
## Comment arrêter, redémarrer, et finalement supprimer un conteneur et une image?
```bash
docker stop f3bb8db84b52
```
```bash
docker restart f3bb8db84b52
```
```bash
docker rm f3bb8db84b52
```
