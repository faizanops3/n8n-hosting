```
docker exec -u 0 -it n8n sh
npm install -g lodash
exit
```

### Option 2: Best Practice — Build a custom Docker image

```
FROM docker.n8n.io/n8nio/n8n:latest

USER root
RUN npm install -g lodash
USER node
```

write a bash script to take a backup and restore
when this script will be executed , it will ask what do you want to do 1. backup or 2. restore

lets use everything whihc is recomended ,

it will ask the name of container in which this postgres database is running
then it will ask for database credentials like, POSTGRES_USER, POSTGRES_PASSWORD, POSTGRES_DB

then is save the backup where this script is in the same location.
