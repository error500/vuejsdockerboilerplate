### Boilerplate VueJS Docker
Starter kit pour VueJS / docker sous Docker desktop Windows

## Initialisation

Sous Powershell

```
mkdir myproject

cd myproject

docker run --rm -v ${PWD}/dev:/app/dev -w /app/dev -it node:11.1-alpine sh -c "yarn global add @vue/cli && vue create ."
```

Sélectionner yarn comme gestionnaire de dépendances

## lancer le serveur
```
docker run --rm -v ${PWD}/dev:/app/dev -p 8080:8080 -w /app/dev -it node:11.1-alpine sh -c "yarn serve"
```

## Build 
```
docker run --rm -v ${PWD}/dev:/app/dev -p 8080:8080 -w /app/dev -it node:11.1-alpine sh -c "yarn build"
```


## Développement

```
docker-compose up
```
