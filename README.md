# Docker Gitlab

## Use

Two ways:

* Just execute `./gitlab` for a simple container
* Use a Docker stack:

```bash
echo "my_awesome_password" | docker secret create gitlab_root_password -
docker stack deploy -c docker-compose.yml gitlab
```
