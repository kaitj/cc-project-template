# {{ cookiecutter.project_name }}

## Installation

{{ cookiecutter.project_name }} can be installed directly via `pip` or by first
cloning the repository (for development)

### Direct

```bash
pip install {{ cookiecutter.__project_slug }}
```

### For development

```bash
git clone https://github.com/{{ cookiecutter.github }}/{{ cookiecutter.__project_slug }}
cd {{ cookiecutter.__project_slug }}
pip install -e .
```

## Contributing

{{ cookiecutter.project_name }} is an open-source project and contributions
are welcome! If you have any bug reports, feature requests, or improvements,
please submit them to the issues page.

To contribute, first clone the Github repository.
{{ cookiecutter.project_name }} dependencies are managed with [Poetry].
Please refer to the Poetry website for installation instructions.

_Note: {{ cookiecutter.project_name }} makes use of Poetry's dynamic
versioning. To see a version number on locally installed
{{ cookiecutter.project_name }}, you will have to also install
`poetry-dynamic-versioning` plugin to your poetry installation
(`poetry self add "poetry-dynamic-versioning[plugin]").
This is not required for contribution._

Following installation of Poetry, the development can be set up by running the
following command.

```bash
poetry install
```

{{ cookiecutter.project_name }} uses `poethepoet` as a task runner.
You can see what commands are available by running:

```bash
poetry run poe
```

Tests are done with pytest and can be run via:

```bash
poetry run poe test
```

Additionally, {{ cookiecutter.project_name }} uses `yamlfix`, `isort`, `black`,
and `ruff` to lint and format code. These checks are in place for every pull
request made. To fix your code locally, you can run the follow task:

```bash
poetry run poe quality
```

## License

{{ cookiecutter.project_name }} is distributed under the
{{ cookiecutter.license}} license.

[Poetry]: https://python-poetry.org/
