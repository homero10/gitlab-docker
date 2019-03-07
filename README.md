# Docker Gitlab

## Use

Two ways:

* Just execute `./gitlab` for a simple container
* Use a Docker stack. First, create a password as a secret (one-time command):

```bash
echo "my_awesome_password" | docker secret create gitlab_root_password -
```

* Then, deploy the stack:

```bash
docker stack deploy -c docker-compose.yml gitlab
```
