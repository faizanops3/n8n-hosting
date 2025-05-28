## For terafik with docker swarm

- Add domain in .env
- run this command

```
docker stack deploy -c new-my-setup-terrafik-swarm-frappe/n8n-stack.yml n8n
```

---

```
docker stack rm new-my-setup-terrafik-swarm-frappe/n8n-stack.yml n8n
```
