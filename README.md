### Boilerplate VueJS Docker
Starter kit pour VueJS / docker sous Docker desktop Windows

## Initialisation

Sous Powershell

```
mkdir myproject

cd myproject

docker run --rm -v ${PWD}:/app -w /app -it node:11.1-alpine sh -c "yarn global add @vue/cli && vue create ."
```


Sélectionner yarn comme gestionnaire de dépendances

voir éventuellement avec "-d" pour les defaults
```
docker run --rm -v ${PWD}:/app -w /app -it node:11.1-alpine sh -c "yarn global add @vue/cli && vue create . -d"
```

## Développement

```
docker-compose up
```

