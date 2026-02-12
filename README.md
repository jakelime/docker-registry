# title

## Troubleshoots

### Exec into broken containers

```bash
docker compose run --rm --entrypoint /bin/sh nginx
```

## Quickstart

```bash
# Pull an example image
docker pull alpine
# Tag the image
docker tag alpine localhost:10500/my-alpine
# Push the image into the self-hosted instance
docker push localhost:10500/my-alpine
```
