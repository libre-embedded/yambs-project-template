<!--
    =====================================
    generator=datazen
    version=3.2.4
    hash=55da3ca12886610c6c3821dfcb094f3a
    =====================================
-->

# yambs-project-template

![Build Status](https://github.com/libre-embedded/yambs-project-template/actions/workflows/create-project.yml/badge.svg)

The [yambs](https://github.com/libre-embedded/yambs) project implements a C/C++
build-system.

*This is a template intended to be used with
[Cookiecutter](https://github.com/cookiecutter/cookiecutter).*

# Usage

Invoke `cookiecutter` and fill out information about your project:

```
cookiecutter git@github.com:libre-embedded/yambs-project-template.git
```

Example output (interactive):

```
name [Libre Embedded]: <Your Name>
email [vaughn@libre-embedded.com]: <your@email.com>
...
```

## Structure

```
$ tree -a -I venv*|__pycache__|dist|*cov*|*-out|config|ninja|.ninja*|build|*.egg-info|tags|mklocal|.git*|.*cache*|third-party|docs|toolchains -- project-name

project-name
├── build.ninja
├── .clang-format
├── compile_commands.json
├── ifgen.yaml
├── .isort.cfg
├── LICENSE
├── local
│   ├── configs
│   │   ├── license.yaml
│   │   └── project.yaml
│   └── yambs.yaml
├── Makefile
├── manifest.yaml
├── mypy.ini
├── project_name
│   ├── __init__.py
│   └── requirements.txt
├── README.md
├── src
│   ├── apps
│   │   ├── generated
│   │   │   └── ifgen
│   │   │       └── test_common.cc
│   │   └── test_file.cc
│   ├── example
│   │   ├── sample.cc
│   │   └── sample.h
│   └── generated
│       ├── custom
│       │   └── struct_receiver.h
│       └── ifgen
│           └── common.h
├── tasks
│   └── conf.py
└── yambs.yaml

13 directories, 23 files

```
