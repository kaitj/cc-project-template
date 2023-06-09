# Cookiecutter Project Template

A cookiecutter template for Python projects using Poetry.

## Features

- [Poetry](https://python-poetry.org/) project management
- Automated versioning with Poetry's dynamic versioning
- Issue and PR templates
- Linting and formatting (`yamlfix`,`isort`, `black`, `ruff`)
- Unit-testing (`pytest`, `hypothesis`)
- Code coverage (`codecov`)
- [Release drafter](https://github.com/marketplace/actions/release-drafter)

## Usage

`cookiecutter` will need to be installed.

```
pip install cookiecutter
```

Once installed, this template can be used to automatically set up future
projects:

```
cookiecutter gh:kaitj/cc-project-template
```

Once this is setup, a few additional tasks need to be performed to set up some
of the tools (see the checklist).

### Checklist

- Setup Github repo if not already done
- Add environment secrets
  - PyPI API token (for publishing)
  - Project-specific github access token (saved as `BP_PAT_TOKEN`)
  - `Codecov` token (for uploading reports on PR, free for public repos)
- Add reviewers for auto-assignment on new PRs
- Setup documentation (e.g. [readthedocs](https://readthedocs.org))
