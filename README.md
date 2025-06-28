[![add-on registry](https://img.shields.io/badge/DDEV-Add--on_Registry-blue)](https://addons.ddev.com)
[![tests](https://github.com/egemasta/ddev-codeigniter4/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/egemasta/ddev-codeigniter4/actions/workflows/tests.yml?query=branch%3Amain)
[![last commit](https://img.shields.io/github/last-commit/egemasta/ddev-codeigniter4)](https://github.com/egemasta/ddev-codeigniter4/commits)
[![release](https://img.shields.io/github/v/release/egemasta/ddev-codeigniter4)](https://github.com/egemasta/ddev-codeigniter4/releases/latest)

# DDEV Codeigniter4

## Overview

This add-on integrates Codeigniter4 into your [DDEV](https://ddev.com/) project.

## Installation

```bash
ddev add-on get egemasta/ddev-codeigniter4
ddev restart
```

After installation, make sure to commit the `.ddev` directory to version control.

## Usage

| Command | Description |
| ------- | ----------- |
| `ddev describe` | View service status and used ports for Codeigniter4 |
| `ddev logs -s codeigniter4` | Check Codeigniter4 logs |

## Advanced Customization

To change the Docker image:

```bash
ddev dotenv set .ddev/.env.codeigniter4 --codeigniter4-docker-image="busybox:stable"
ddev add-on get egemasta/ddev-codeigniter4
ddev restart
```

Make sure to commit the `.ddev/.env.codeigniter4` file to version control.

All customization options (use with caution):

| Variable | Flag | Default |
| -------- | ---- | ------- |
| `CODEIGNITER4_DOCKER_IMAGE` | `--codeigniter4-docker-image` | `busybox:stable` |

## Credits

**Contributed and maintained by [@egemasta](https://github.com/egemasta)**
