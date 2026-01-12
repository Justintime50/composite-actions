# Composite Actions

A collection of composite GitHub Actions used in my projects.

## Usage

### PHP

Checks out the repo, installs PHP (use `php-version` input), installs Node (use `node-version` input), and installs `just`.

```yml
- uses: justintime50/composite-actions/bootstrap-php@v1
```

### Python

Checks out the repo, install Python (use `python-version` input), and installs `just`.

```yml
- uses: justintime50/composite-actions/bootstrap-python@v1
```
