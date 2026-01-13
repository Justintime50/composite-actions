# Composite Actions

A collection of composite GitHub Actions used in my projects.

> NOTE: These actions are intended for my own personal use as they are customized to me. I will not be accepting contributions. These should not be used directly for your projects.

## Usage

### Docker

Checks out the repo, sets up `qemu`/`buildx`, signs into Docker, builds image, and pushes to registry.

```yml
# Private Registry
- uses: justintime50/composite-actions/publish-private-image@v1

# Docker Hub
- uses: justintime50/composite-actions/publish-public-image@v1
```

### PHP

Checks out the repo, installs PHP (use `php-version` input), installs Node (use `node-version` input), installs `just`, and sets up a `traefik` Docker network.

```yml
- uses: justintime50/composite-actions/bootstrap-php@v1
```

### Python

Checks out the repo, install Python (use `python-version` input), installs `just`, and installs `uv`.

```yml
- uses: justintime50/composite-actions/bootstrap-python@v1
```
