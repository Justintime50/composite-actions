# Composite Actions

A collection of composite GitHub Actions used in my projects.

## Usage

### Docker

Checks out the repo, sets up `qemu`, signs into Docker, builds image, and pushes to registry.

```yml
- uses: justintime50/composite-actions/publish-docker@v1
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
