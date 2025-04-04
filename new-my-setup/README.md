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
