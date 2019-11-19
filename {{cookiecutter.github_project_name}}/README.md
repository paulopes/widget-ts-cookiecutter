
# {{ cookiecutter.github_project_name }}

[![Build Status](https://travis-ci.org/{{ cookiecutter.github_organization_name }}/{{ cookiecutter.github_project_name  }}.svg?branch=master)](https://travis-ci.org/{{ cookiecutter.github_organization_name }}/{{ cookiecutter.python_package_name  }})
[![codecov](https://codecov.io/gh/{{ cookiecutter.github_organization_name }}/{{ cookiecutter.github_project_name  }}/branch/master/graph/badge.svg)](https://codecov.io/gh/{{ cookiecutter.github_organization_name }}/{{ cookiecutter.github_project_name  }})


{{ cookiecutter.project_short_description }}

## Installation

You can install using `pip`:

```bash
pip install {{ cookiecutter.python_package_name  }}
```

Install the Jupyter Notebook extension:
```bash
jupyter nbextension enable --py --sys-prefix {{ cookiecutter.python_package_name  }}
```

If you use JupyterLab:

Make sure that JupyterLab Manager is installed:
```bash
jupyter labextension install @jupyter-widgets/jupyterlab-manager
```

Install the JupyterLab extension:
```bash
jupyter labextension install {{ cookiecutter.python_package_name  }}
```

For a development installation (requires npm),

```bash
git clone https://github.com/{{ cookiecutter.github_organization_name  }}/{{ cookiecutter.github_project_name }}.git
cd {{ cookiecutter.github_project_name }}
pip install -e .
jupyter nbextension install --py --symlink --sys-prefix {{ cookiecutter.python_package_name }}
jupyter nbextension enable --py --sys-prefix {{ cookiecutter.python_package_name }}
jupyter labextension install
```

When actively developing your extension, build Jupyter Lab with the command:

```bash
jupyter lab --watch
```

This take a minute or so to get started, but then allows you to hot-reload your javascript extension.
To see a change, save your javascript, watch the terminal for an update.

Note on first `jupyter lab --watch`, you may need to touch a file to get Jupyter Lab to open.
