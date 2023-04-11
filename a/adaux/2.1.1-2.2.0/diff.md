# Comparing `tmp/adaux-2.1.1.tar.gz` & `tmp/adaux-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adaux-2.1.1.tar", last modified: Tue Apr  4 14:59:12 2023, max compression
+gzip compressed data, was "adaux-2.2.0.tar", last modified: Tue Apr 11 12:41:58 2023, max compression
```

## Comparing `adaux-2.1.1.tar` & `adaux-2.2.0.tar`

### file list

```diff
@@ -1,151 +1,151 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 14:59:12.951686 adaux-2.1.1/
--rw-rw-rw-   0 root         (0) root         (0)     1059 2023-04-04 14:24:51.000000 adaux-2.1.1/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      314 2023-04-04 14:59:12.951686 adaux-2.1.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      919 2023-04-04 14:59:12.955686 adaux-2.1.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      144 2022-07-30 13:12:02.000000 adaux-2.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 14:59:12.827682 adaux-2.1.1/source/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 14:59:12.859683 adaux-2.1.1/source/adaux/
--rw-rw-rw-   0 root         (0) root         (0)      302 2023-04-04 14:24:51.000000 adaux-2.1.1/source/adaux/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      978 2023-04-04 14:24:51.000000 adaux-2.1.1/source/adaux/_base_parser.py
--rw-rw-rw-   0 root         (0) root         (0)    13482 2023-04-04 14:24:51.000000 adaux-2.1.1/source/adaux/_cli.py
--rw-rw-rw-   0 root         (0) root         (0)    14078 2023-04-04 14:24:51.000000 adaux-2.1.1/source/adaux/_cli_mixin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 14:59:12.887684 adaux-2.1.1/source/adaux/_components/
--rw-rw-rw-   0 root         (0) root         (0)      229 2023-04-04 14:24:51.000000 adaux-2.1.1/source/adaux/_components/_00_extra_level.py
--rw-rw-rw-   0 root         (0) root         (0)     4879 2023-04-04 14:24:51.000000 adaux-2.1.1/source/adaux/_components/_01_file_io_support.py
--rw-rw-rw-   0 root         (0) root         (0)     4867 2023-04-04 14:24:51.000000 adaux-2.1.1/source/adaux/_components/_02_base.py
--rw-rw-rw-   0 root         (0) root         (0)     3208 2023-04-04 14:24:51.000000 adaux-2.1.1/source/adaux/_components/_03_meta.py
--rw-rw-rw-   0 root         (0) root         (0)     1471 2023-04-04 14:24:51.000000 adaux-2.1.1/source/adaux/_components/_04_monotonic_version.py
--rw-rw-rw-   0 root         (0) root         (0)     6617 2023-04-04 14:24:51.000000 adaux-2.1.1/source/adaux/_components/_05_project.py
--rw-rw-rw-   0 root         (0) root         (0)     4528 2023-04-04 14:24:51.000000 adaux-2.1.1/source/adaux/_components/_06_dependency.py
--rw-rw-rw-   0 root         (0) root         (0)     1192 2023-04-04 14:24:51.000000 adaux-2.1.1/source/adaux/_components/_07_package.py
--rw-rw-rw-   0 root         (0) root         (0)     3629 2023-04-04 14:24:51.000000 adaux-2.1.1/source/adaux/_components/_08_pip.py
--rw-rw-rw-   0 root         (0) root         (0)     1888 2023-04-04 14:24:51.000000 adaux-2.1.1/source/adaux/_components/_09_gitignore.py
--rw-rw-rw-   0 root         (0) root         (0)     3847 2023-04-04 14:24:51.000000 adaux-2.1.1/source/adaux/_components/_10_gitlab.py
--rw-rw-rw-   0 root         (0) root         (0)     5765 2023-04-04 14:24:51.000000 adaux-2.1.1/source/adaux/_components/_11_precommit.py
--rw-rw-rw-   0 root         (0) root         (0)     5202 2023-04-04 14:41:03.000000 adaux-2.1.1/source/adaux/_components/_12_pylint.py
--rw-rw-rw-   0 root         (0) root         (0)     1408 2023-04-04 14:24:51.000000 adaux-2.1.1/source/adaux/_components/_13_executable.py
--rw-rw-rw-   0 root         (0) root         (0)     2257 2023-04-04 14:24:51.000000 adaux-2.1.1/source/adaux/_components/_14_mypy.py
--rw-rw-rw-   0 root         (0) root         (0)     2413 2023-04-04 14:24:51.000000 adaux-2.1.1/source/adaux/_components/_15_pytest.py
--rw-rw-rw-   0 root         (0) root         (0)      292 2023-04-04 14:24:51.000000 adaux-2.1.1/source/adaux/_components/_16_coverage.py
--rw-rw-rw-   0 root         (0) root         (0)     2753 2023-04-04 14:24:51.000000 adaux-2.1.1/source/adaux/_components/_17_docs.py
--rw-rw-rw-   0 root         (0) root         (0)    15582 2023-04-04 14:24:51.000000 adaux-2.1.1/source/adaux/_components/_18_payload.py
--rw-rw-rw-   0 root         (0) root         (0)    15504 2023-04-04 14:24:51.000000 adaux-2.1.1/source/adaux/_components/_19_docker.py
--rw-rw-rw-   0 root         (0) root         (0)    10820 2023-04-04 14:24:51.000000 adaux-2.1.1/source/adaux/_components/_20_ci.py
--rw-rw-rw-   0 root         (0) root         (0)     2524 2023-04-04 14:24:51.000000 adaux-2.1.1/source/adaux/_components/_98_sentinel.py
--rw-rw-rw-   0 root         (0) root         (0)     1221 2023-04-04 14:24:51.000000 adaux-2.1.1/source/adaux/_components/_99_all.py
--rw-rw-rw-   0 root         (0) root         (0)      215 2023-04-04 14:24:51.000000 adaux-2.1.1/source/adaux/_components/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12817 2023-04-04 14:24:51.000000 adaux-2.1.1/source/adaux/_components/_aux_ci.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 14:59:12.903684 adaux-2.1.1/source/adaux/_components/_payload/
--rw-rw-rw-   0 root         (0) root         (0)      612 2023-04-04 14:24:51.000000 adaux-2.1.1/source/adaux/_components/_payload/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      530 2023-04-04 14:24:51.000000 adaux-2.1.1/source/adaux/_components/_payload/_base.py
--rw-rw-rw-   0 root         (0) root         (0)     1618 2023-04-04 14:24:51.000000 adaux-2.1.1/source/adaux/_components/_payload/_docker.py
--rw-rw-rw-   0 root         (0) root         (0)      806 2023-04-04 14:24:51.000000 adaux-2.1.1/source/adaux/_components/_payload/_docker_build.py
--rw-rw-rw-   0 root         (0) root         (0)      382 2023-04-04 14:24:51.000000 adaux-2.1.1/source/adaux/_components/_payload/_docker_compose.py
--rw-rw-rw-   0 root         (0) root         (0)    15321 2023-04-04 14:24:51.000000 adaux-2.1.1/source/adaux/_components/_payload/_docker_executors.py
--rw-rw-rw-   0 root         (0) root         (0)      547 2023-04-04 14:24:51.000000 adaux-2.1.1/source/adaux/_components/_payload/_docker_run.py
--rw-rw-rw-   0 root         (0) root         (0)     1450 2023-04-04 14:24:51.000000 adaux-2.1.1/source/adaux/_components/_payload/_python.py
--rw-rw-rw-   0 root         (0) root         (0)     1358 2023-04-04 14:24:51.000000 adaux-2.1.1/source/adaux/_components/_payload/_with_dependency.py
--rwxrwxrwx   0 root         (0) root         (0)     1629 2023-04-04 14:24:51.000000 adaux-2.1.1/source/adaux/_create_badge.py
--rw-rw-rw-   0 root         (0) root         (0)    14534 2023-04-04 14:24:51.000000 adaux-2.1.1/source/adaux/_gitlab.py
--rw-rw-rw-   0 root         (0) root         (0)      107 2023-04-04 14:24:51.000000 adaux-2.1.1/source/adaux/_logging.py
--rw-rw-rw-   0 root         (0) root         (0)     7082 2023-04-04 14:24:51.000000 adaux-2.1.1/source/adaux/_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     1245 2023-04-04 14:24:51.000000 adaux-2.1.1/source/adaux/_proto_namespace.py
--rw-rw-rw-   0 root         (0) root         (0)     2464 2023-04-04 14:24:51.000000 adaux-2.1.1/source/adaux/_tick.py
--rw-rw-rw-   0 root         (0) root         (0)     3388 2023-04-04 14:24:51.000000 adaux-2.1.1/source/adaux/_todo.py
--rw-rw-rw-   0 root         (0) root         (0)     2751 2023-04-04 14:24:51.000000 adaux-2.1.1/source/adaux/_util.py
--rw-rw-rw-   0 root         (0) root         (0)      329 2023-04-04 14:24:51.000000 adaux-2.1.1/source/adaux/_yaml.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-04 14:24:51.000000 adaux-2.1.1/source/adaux/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 14:59:12.907684 adaux-2.1.1/source/adaux/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 14:59:12.911685 adaux-2.1.1/source/adaux/src/CI/
--rw-rw-rw-   0 root         (0) root         (0)     2316 2023-04-04 14:24:51.000000 adaux-2.1.1/source/adaux/src/CI/00-main.yml.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      922 2023-04-04 14:24:51.000000 adaux-2.1.1/source/adaux/src/CI/01-rules.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 14:59:12.911685 adaux-2.1.1/source/adaux/src/CI/jinja-snippets/
--rw-rw-rw-   0 root         (0) root         (0)       50 2023-04-04 14:24:51.000000 adaux-2.1.1/source/adaux/src/CI/jinja-snippets/coverage.jinja2
--rw-rw-rw-   0 root         (0) root         (0)       94 2023-04-04 14:24:51.000000 adaux-2.1.1/source/adaux/src/CI/jinja-snippets/tags.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 14:59:12.911685 adaux-2.1.1/source/adaux/src/docker/
--rw-rw-rw-   0 root         (0) root         (0)      417 2023-04-04 14:24:51.000000 adaux-2.1.1/source/adaux/src/docker/comp-helper.sh.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 14:59:12.839682 adaux-2.1.1/source/adaux/src/docker/services/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 14:59:12.915685 adaux-2.1.1/source/adaux/src/docker/services/ansible-deploy/
--rw-rw-rw-   0 root         (0) root         (0)      914 2023-04-04 14:24:51.000000 adaux-2.1.1/source/adaux/src/docker/services/ansible-deploy/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      547 2023-04-04 14:24:51.000000 adaux-2.1.1/source/adaux/src/docker/services/ansible-deploy/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 14:59:12.915685 adaux-2.1.1/source/adaux/src/docker/services/docs/
--rw-rw-rw-   0 root         (0) root         (0)     1385 2023-04-04 14:24:51.000000 adaux-2.1.1/source/adaux/src/docker/services/docs/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      459 2023-04-04 14:24:51.000000 adaux-2.1.1/source/adaux/src/docker/services/docs/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 14:59:12.919685 adaux-2.1.1/source/adaux/src/docker/services/gitlab-release-run/
--rw-rw-rw-   0 root         (0) root         (0)      608 2023-04-04 14:24:51.000000 adaux-2.1.1/source/adaux/src/docker/services/gitlab-release-run/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 14:59:12.919685 adaux-2.1.1/source/adaux/src/docker/services/image/
--rw-rw-rw-   0 root         (0) root         (0)     1564 2023-04-04 14:24:51.000000 adaux-2.1.1/source/adaux/src/docker/services/image/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      407 2023-04-04 14:24:51.000000 adaux-2.1.1/source/adaux/src/docker/services/image/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 14:59:12.919685 adaux-2.1.1/source/adaux/src/docker/services/image-pytest/
--rw-rw-rw-   0 root         (0) root         (0)      617 2023-04-04 14:24:51.000000 adaux-2.1.1/source/adaux/src/docker/services/image-pytest/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      365 2023-04-04 14:24:51.000000 adaux-2.1.1/source/adaux/src/docker/services/image-pytest/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 14:59:12.927685 adaux-2.1.1/source/adaux/src/docker/services/jinja-snippets/
--rw-rw-rw-   0 root         (0) root         (0)      505 2023-04-04 14:24:51.000000 adaux-2.1.1/source/adaux/src/docker/services/jinja-snippets/apt_install.jinja2
--rw-rw-rw-   0 root         (0) root         (0)       87 2023-04-04 14:24:51.000000 adaux-2.1.1/source/adaux/src/docker/services/jinja-snippets/apt_install_root.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-04-04 14:24:51.000000 adaux-2.1.1/source/adaux/src/docker/services/jinja-snippets/base_arg.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      529 2023-04-04 14:24:51.000000 adaux-2.1.1/source/adaux/src/docker/services/jinja-snippets/docker-build.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      169 2023-04-04 14:24:52.000000 adaux-2.1.1/source/adaux/src/docker/services/jinja-snippets/extra_script.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      437 2023-04-04 14:24:52.000000 adaux-2.1.1/source/adaux/src/docker/services/jinja-snippets/macros.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      326 2023-04-04 14:24:52.000000 adaux-2.1.1/source/adaux/src/docker/services/jinja-snippets/pip_install.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      113 2023-04-04 14:24:52.000000 adaux-2.1.1/source/adaux/src/docker/services/jinja-snippets/platform.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      247 2023-04-04 14:24:52.000000 adaux-2.1.1/source/adaux/src/docker/services/jinja-snippets/pytest_command.jinja2
--rw-rw-rw-   0 root         (0) root         (0)       58 2023-04-04 14:24:52.000000 adaux-2.1.1/source/adaux/src/docker/services/jinja-snippets/sdist_untar.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 14:59:12.927685 adaux-2.1.1/source/adaux/src/docker/services/pkg-gitlab/
--rw-rw-rw-   0 root         (0) root         (0)      547 2023-04-04 14:24:52.000000 adaux-2.1.1/source/adaux/src/docker/services/pkg-gitlab/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 14:59:12.931685 adaux-2.1.1/source/adaux/src/docker/services/pkg-pypi/
--rw-rw-rw-   0 root         (0) root         (0)      485 2023-04-04 14:24:52.000000 adaux-2.1.1/source/adaux/src/docker/services/pkg-pypi/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 14:59:12.931685 adaux-2.1.1/source/adaux/src/docker/services/pre-commit/
--rw-rw-rw-   0 root         (0) root         (0)     1107 2023-04-04 14:24:52.000000 adaux-2.1.1/source/adaux/src/docker/services/pre-commit/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      599 2023-04-04 14:24:52.000000 adaux-2.1.1/source/adaux/src/docker/services/pre-commit/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 14:59:12.931685 adaux-2.1.1/source/adaux/src/docker/services/pycov/
--rw-rw-rw-   0 root         (0) root         (0)      482 2023-04-04 14:24:52.000000 adaux-2.1.1/source/adaux/src/docker/services/pycov/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 14:59:12.935685 adaux-2.1.1/source/adaux/src/docker/services/pytest/
--rw-rw-rw-   0 root         (0) root         (0)      342 2023-04-04 14:24:52.000000 adaux-2.1.1/source/adaux/src/docker/services/pytest/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      409 2023-04-04 14:24:52.000000 adaux-2.1.1/source/adaux/src/docker/services/pytest/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 14:59:12.935685 adaux-2.1.1/source/adaux/src/docker/services/pytest-standalone/
--rw-rw-rw-   0 root         (0) root         (0)      569 2023-04-04 14:24:52.000000 adaux-2.1.1/source/adaux/src/docker/services/pytest-standalone/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      409 2023-04-04 14:24:52.000000 adaux-2.1.1/source/adaux/src/docker/services/pytest-standalone/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 14:59:12.935685 adaux-2.1.1/source/adaux/src/docker/services/python-deps/
--rw-rw-rw-   0 root         (0) root         (0)      648 2023-04-04 14:24:52.000000 adaux-2.1.1/source/adaux/src/docker/services/python-deps/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      211 2023-04-04 14:24:52.000000 adaux-2.1.1/source/adaux/src/docker/services/python-deps/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 14:59:12.939686 adaux-2.1.1/source/adaux/src/docs/
--rw-rw-rw-   0 root         (0) root         (0)     4843 2023-04-04 14:24:52.000000 adaux-2.1.1/source/adaux/src/docs/default_conf.py.jinja2
--rwxrwxrwx   0 root         (0) root         (0)     1873 2023-04-04 14:24:52.000000 adaux-2.1.1/source/adaux/src/docs/postprocess_html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 14:59:12.939686 adaux-2.1.1/source/adaux/src/docs/static/
--rw-rw-rw-   0 root         (0) root         (0)       72 2023-04-04 14:24:52.000000 adaux-2.1.1/source/adaux/src/docs/static/git-link-color.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 14:59:12.943686 adaux-2.1.1/source/adaux/src/docs/user/
--rw-rw-rw-   0 root         (0) root         (0)      468 2023-04-04 14:24:52.000000 adaux-2.1.1/source/adaux/src/docs/user/conf.py.jinja2
--rw-rw-rw-   0 root         (0) root         (0)       45 2023-04-04 14:24:52.000000 adaux-2.1.1/source/adaux/src/docs/user/gitignore
--rw-rw-rw-   0 root         (0) root         (0)      283 2023-04-04 14:24:52.000000 adaux-2.1.1/source/adaux/src/docs/user/index.rst.jinja2
--rw-rw-rw-   0 root         (0) root         (0)       45 2023-04-04 14:24:52.000000 adaux-2.1.1/source/adaux/src/gitignore
--rwxrwxrwx   0 root         (0) root         (0)      410 2023-04-04 14:24:52.000000 adaux-2.1.1/source/adaux/src/install-dev.sh.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 14:59:12.943686 adaux-2.1.1/source/adaux/src/license/
--rw-rw-rw-   0 root         (0) root         (0)      591 2023-04-04 14:24:52.000000 adaux-2.1.1/source/adaux/src/license/Apache-2.0.txt.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     1495 2023-04-04 14:24:52.000000 adaux-2.1.1/source/adaux/src/license/BSD-3_clause.txt.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     1090 2023-04-04 14:24:52.000000 adaux-2.1.1/source/adaux/src/license/MIT.txt.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 14:59:12.843682 adaux-2.1.1/source/adaux/src/payload/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 14:59:12.947686 adaux-2.1.1/source/adaux/src/payload/python/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 14:59:12.947686 adaux-2.1.1/source/adaux/src/payload/python/__pycache__/
--rw-r--r--   0 root         (0) root         (0)     2428 2023-04-04 14:58:11.000000 adaux-2.1.1/source/adaux/src/payload/python/__pycache__/functions.cpython-310.pyc
--rw-rw-rw-   0 root         (0) root         (0)     2816 2023-04-04 14:24:52.000000 adaux-2.1.1/source/adaux/src/payload/python/functions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 14:59:12.947686 adaux-2.1.1/source/adaux/src/pip/
--rw-rw-rw-   0 root         (0) root         (0)      160 2023-04-04 14:24:52.000000 adaux-2.1.1/source/adaux/src/pip/pip.conf.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 14:59:12.951686 adaux-2.1.1/source/adaux/src/pre-commit/
--rwxrwxrwx   0 root         (0) root         (0)     1680 2023-04-04 14:24:52.000000 adaux-2.1.1/source/adaux/src/pre-commit/add_copy_right.py.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     5098 2023-04-04 14:24:52.000000 adaux-2.1.1/source/adaux/src/pre-commit/config.yaml.jinja2
--rw-rw-rw-   0 root         (0) root         (0)       84 2023-04-04 14:24:52.000000 adaux-2.1.1/source/adaux/src/pre-commit/mypy.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 14:59:12.951686 adaux-2.1.1/source/adaux/src/root/
--rw-rw-rw-   0 root         (0) root         (0)      144 2023-04-04 14:24:52.000000 adaux-2.1.1/source/adaux/src/root/_setup.py
--rw-rw-rw-   0 root         (0) root         (0)      146 2023-04-04 14:24:52.000000 adaux-2.1.1/source/adaux/src/root/gitignore.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      487 2023-04-04 14:24:52.000000 adaux-2.1.1/source/adaux/src/root/setup.cfg.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 14:59:12.951686 adaux-2.1.1/source/adaux/src/root/source/
--rw-rw-rw-   0 root         (0) root         (0)      126 2023-04-04 14:24:52.000000 adaux-2.1.1/source/adaux/src/root/source/gitignore.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      127 2023-04-04 14:24:52.000000 adaux-2.1.1/source/adaux/src/temp-combination
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 14:59:12.867683 adaux-2.1.1/source/adaux.egg-info/
--rw-r--r--   0 root         (0) root         (0)      314 2023-04-04 14:59:12.000000 adaux-2.1.1/source/adaux.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5236 2023-04-04 14:59:12.000000 adaux-2.1.1/source/adaux.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-04 14:59:12.000000 adaux-2.1.1/source/adaux.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-04-04 14:59:12.000000 adaux-2.1.1/source/adaux.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-04 14:58:10.000000 adaux-2.1.1/source/adaux.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      203 2023-04-04 14:59:12.000000 adaux-2.1.1/source/adaux.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-04-04 14:59:12.000000 adaux-2.1.1/source/adaux.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.881155 adaux-2.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1059 2023-04-10 20:31:51.000000 adaux-2.2.0/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      314 2023-04-11 12:41:58.881155 adaux-2.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1030 2023-04-11 12:41:58.881155 adaux-2.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      144 2022-07-30 13:12:02.000000 adaux-2.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.713149 adaux-2.2.0/source/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.805153 adaux-2.2.0/source/adaux/
+-rw-rw-rw-   0 root         (0) root         (0)      302 2023-04-11 12:31:50.000000 adaux-2.2.0/source/adaux/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      978 2023-04-10 20:31:51.000000 adaux-2.2.0/source/adaux/_base_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)    13574 2023-04-10 20:31:51.000000 adaux-2.2.0/source/adaux/_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    14120 2023-04-10 20:31:51.000000 adaux-2.2.0/source/adaux/_cli_mixin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.833154 adaux-2.2.0/source/adaux/_components/
+-rw-rw-rw-   0 root         (0) root         (0)      229 2023-04-10 20:31:51.000000 adaux-2.2.0/source/adaux/_components/_00_extra_level.py
+-rw-rw-rw-   0 root         (0) root         (0)     4879 2023-04-10 20:31:51.000000 adaux-2.2.0/source/adaux/_components/_01_file_io_support.py
+-rw-rw-rw-   0 root         (0) root         (0)     4867 2023-04-10 20:31:51.000000 adaux-2.2.0/source/adaux/_components/_02_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3208 2023-04-10 20:31:51.000000 adaux-2.2.0/source/adaux/_components/_03_meta.py
+-rw-rw-rw-   0 root         (0) root         (0)     1471 2023-04-10 20:31:51.000000 adaux-2.2.0/source/adaux/_components/_04_monotonic_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     6617 2023-04-10 20:31:51.000000 adaux-2.2.0/source/adaux/_components/_05_project.py
+-rw-rw-rw-   0 root         (0) root         (0)     4979 2023-04-10 21:56:59.000000 adaux-2.2.0/source/adaux/_components/_06_dependency.py
+-rw-rw-rw-   0 root         (0) root         (0)     1192 2023-04-10 20:31:51.000000 adaux-2.2.0/source/adaux/_components/_07_package.py
+-rw-rw-rw-   0 root         (0) root         (0)     3686 2023-04-10 20:31:51.000000 adaux-2.2.0/source/adaux/_components/_08_pip.py
+-rw-rw-rw-   0 root         (0) root         (0)     1888 2023-04-10 20:31:51.000000 adaux-2.2.0/source/adaux/_components/_09_gitignore.py
+-rw-rw-rw-   0 root         (0) root         (0)     4087 2023-04-10 20:31:51.000000 adaux-2.2.0/source/adaux/_components/_10_gitlab.py
+-rw-rw-rw-   0 root         (0) root         (0)     5765 2023-04-10 20:31:51.000000 adaux-2.2.0/source/adaux/_components/_11_precommit.py
+-rw-rw-rw-   0 root         (0) root         (0)     5277 2023-04-11 12:28:10.000000 adaux-2.2.0/source/adaux/_components/_12_pylint.py
+-rw-rw-rw-   0 root         (0) root         (0)     1473 2023-04-10 20:31:51.000000 adaux-2.2.0/source/adaux/_components/_13_executable.py
+-rw-rw-rw-   0 root         (0) root         (0)     2257 2023-04-10 20:31:51.000000 adaux-2.2.0/source/adaux/_components/_14_mypy.py
+-rw-rw-rw-   0 root         (0) root         (0)     2413 2023-04-10 20:31:51.000000 adaux-2.2.0/source/adaux/_components/_15_pytest.py
+-rw-rw-rw-   0 root         (0) root         (0)      292 2023-04-10 20:31:51.000000 adaux-2.2.0/source/adaux/_components/_16_coverage.py
+-rw-rw-rw-   0 root         (0) root         (0)     2753 2023-04-10 20:31:51.000000 adaux-2.2.0/source/adaux/_components/_17_docs.py
+-rw-rw-rw-   0 root         (0) root         (0)    15797 2023-04-10 20:31:51.000000 adaux-2.2.0/source/adaux/_components/_18_payload.py
+-rw-rw-rw-   0 root         (0) root         (0)    15575 2023-04-11 12:28:10.000000 adaux-2.2.0/source/adaux/_components/_19_docker.py
+-rw-rw-rw-   0 root         (0) root         (0)    10820 2023-04-10 20:31:51.000000 adaux-2.2.0/source/adaux/_components/_20_ci.py
+-rw-rw-rw-   0 root         (0) root         (0)     2524 2023-04-10 20:31:51.000000 adaux-2.2.0/source/adaux/_components/_98_sentinel.py
+-rw-rw-rw-   0 root         (0) root         (0)     1221 2023-04-10 20:31:51.000000 adaux-2.2.0/source/adaux/_components/_99_all.py
+-rw-rw-rw-   0 root         (0) root         (0)      215 2023-04-10 20:31:51.000000 adaux-2.2.0/source/adaux/_components/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12817 2023-04-10 20:31:51.000000 adaux-2.2.0/source/adaux/_components/_aux_ci.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.841154 adaux-2.2.0/source/adaux/_components/_payload/
+-rw-rw-rw-   0 root         (0) root         (0)      612 2023-04-10 20:31:51.000000 adaux-2.2.0/source/adaux/_components/_payload/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      530 2023-04-10 20:31:51.000000 adaux-2.2.0/source/adaux/_components/_payload/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1618 2023-04-10 20:31:51.000000 adaux-2.2.0/source/adaux/_components/_payload/_docker.py
+-rw-rw-rw-   0 root         (0) root         (0)     1077 2023-04-11 12:28:10.000000 adaux-2.2.0/source/adaux/_components/_payload/_docker_build.py
+-rw-rw-rw-   0 root         (0) root         (0)      382 2023-04-10 20:31:51.000000 adaux-2.2.0/source/adaux/_components/_payload/_docker_compose.py
+-rw-rw-rw-   0 root         (0) root         (0)    15703 2023-04-10 20:31:51.000000 adaux-2.2.0/source/adaux/_components/_payload/_docker_executors.py
+-rw-rw-rw-   0 root         (0) root         (0)      490 2023-04-11 12:28:10.000000 adaux-2.2.0/source/adaux/_components/_payload/_docker_run.py
+-rw-rw-rw-   0 root         (0) root         (0)     1450 2023-04-10 20:31:51.000000 adaux-2.2.0/source/adaux/_components/_payload/_python.py
+-rw-rw-rw-   0 root         (0) root         (0)     1358 2023-04-10 20:31:51.000000 adaux-2.2.0/source/adaux/_components/_payload/_with_dependency.py
+-rwxrwxrwx   0 root         (0) root         (0)     1629 2023-04-10 20:31:51.000000 adaux-2.2.0/source/adaux/_create_badge.py
+-rw-rw-rw-   0 root         (0) root         (0)    14742 2023-04-11 12:31:50.000000 adaux-2.2.0/source/adaux/_gitlab.py
+-rw-rw-rw-   0 root         (0) root         (0)      107 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/_logging.py
+-rw-rw-rw-   0 root         (0) root         (0)     7082 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     1245 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/_proto_namespace.py
+-rw-rw-rw-   0 root         (0) root         (0)     2464 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/_tick.py
+-rw-rw-rw-   0 root         (0) root         (0)     3388 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/_todo.py
+-rw-rw-rw-   0 root         (0) root         (0)     2751 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/_util.py
+-rw-rw-rw-   0 root         (0) root         (0)      329 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/_yaml.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.841154 adaux-2.2.0/source/adaux/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.845154 adaux-2.2.0/source/adaux/src/CI/
+-rw-rw-rw-   0 root         (0) root         (0)     2316 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/CI/00-main.yml.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      922 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/CI/01-rules.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.845154 adaux-2.2.0/source/adaux/src/CI/jinja-snippets/
+-rw-rw-rw-   0 root         (0) root         (0)       50 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/CI/jinja-snippets/coverage.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)       94 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/CI/jinja-snippets/tags.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.845154 adaux-2.2.0/source/adaux/src/docker/
+-rw-rw-rw-   0 root         (0) root         (0)      417 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docker/comp-helper.sh.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.749151 adaux-2.2.0/source/adaux/src/docker/services/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.845154 adaux-2.2.0/source/adaux/src/docker/services/ansible-deploy/
+-rw-rw-rw-   0 root         (0) root         (0)      914 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docker/services/ansible-deploy/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      547 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docker/services/ansible-deploy/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.849154 adaux-2.2.0/source/adaux/src/docker/services/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     1385 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docker/services/docs/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      459 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docker/services/docs/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.849154 adaux-2.2.0/source/adaux/src/docker/services/gitlab-release-run/
+-rw-rw-rw-   0 root         (0) root         (0)      608 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docker/services/gitlab-release-run/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.849154 adaux-2.2.0/source/adaux/src/docker/services/image/
+-rw-rw-rw-   0 root         (0) root         (0)     1564 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docker/services/image/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      407 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docker/services/image/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.853155 adaux-2.2.0/source/adaux/src/docker/services/image-pytest/
+-rw-rw-rw-   0 root         (0) root         (0)      617 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docker/services/image-pytest/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      365 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docker/services/image-pytest/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.861155 adaux-2.2.0/source/adaux/src/docker/services/jinja-snippets/
+-rw-rw-rw-   0 root         (0) root         (0)      505 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docker/services/jinja-snippets/apt_install.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)       87 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docker/services/jinja-snippets/apt_install_root.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docker/services/jinja-snippets/base_arg.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      529 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docker/services/jinja-snippets/docker-build.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      169 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docker/services/jinja-snippets/extra_script.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      437 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docker/services/jinja-snippets/macros.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      326 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docker/services/jinja-snippets/pip_install.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      113 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docker/services/jinja-snippets/platform.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      247 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docker/services/jinja-snippets/pytest_command.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)       58 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docker/services/jinja-snippets/sdist_untar.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.861155 adaux-2.2.0/source/adaux/src/docker/services/pkg-gitlab/
+-rw-rw-rw-   0 root         (0) root         (0)      547 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docker/services/pkg-gitlab/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.861155 adaux-2.2.0/source/adaux/src/docker/services/pkg-pypi/
+-rw-rw-rw-   0 root         (0) root         (0)      485 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docker/services/pkg-pypi/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.861155 adaux-2.2.0/source/adaux/src/docker/services/pre-commit/
+-rw-rw-rw-   0 root         (0) root         (0)     1107 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docker/services/pre-commit/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      599 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docker/services/pre-commit/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.861155 adaux-2.2.0/source/adaux/src/docker/services/pycov/
+-rw-rw-rw-   0 root         (0) root         (0)      482 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docker/services/pycov/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.865155 adaux-2.2.0/source/adaux/src/docker/services/pytest/
+-rw-rw-rw-   0 root         (0) root         (0)      342 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docker/services/pytest/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      409 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docker/services/pytest/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.865155 adaux-2.2.0/source/adaux/src/docker/services/pytest-standalone/
+-rw-rw-rw-   0 root         (0) root         (0)      569 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docker/services/pytest-standalone/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      409 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docker/services/pytest-standalone/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.869155 adaux-2.2.0/source/adaux/src/docker/services/python-deps/
+-rw-rw-rw-   0 root         (0) root         (0)      648 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docker/services/python-deps/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      211 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docker/services/python-deps/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.869155 adaux-2.2.0/source/adaux/src/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     4843 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docs/default_conf.py.jinja2
+-rwxrwxrwx   0 root         (0) root         (0)     1873 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docs/postprocess_html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.869155 adaux-2.2.0/source/adaux/src/docs/static/
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docs/static/git-link-color.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.873155 adaux-2.2.0/source/adaux/src/docs/user/
+-rw-rw-rw-   0 root         (0) root         (0)      468 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docs/user/conf.py.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)       45 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docs/user/gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      283 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docs/user/index.rst.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)       45 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/gitignore
+-rwxrwxrwx   0 root         (0) root         (0)      410 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/install-dev.sh.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.873155 adaux-2.2.0/source/adaux/src/license/
+-rw-rw-rw-   0 root         (0) root         (0)      591 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/license/Apache-2.0.txt.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     1495 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/license/BSD-3_clause.txt.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     1090 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/license/MIT.txt.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.757151 adaux-2.2.0/source/adaux/src/payload/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.873155 adaux-2.2.0/source/adaux/src/payload/python/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.873155 adaux-2.2.0/source/adaux/src/payload/python/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)     2601 2023-04-11 12:40:54.000000 adaux-2.2.0/source/adaux/src/payload/python/__pycache__/functions.cpython-310.pyc
+-rw-rw-rw-   0 root         (0) root         (0)     3117 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/payload/python/functions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.877155 adaux-2.2.0/source/adaux/src/pip/
+-rw-rw-rw-   0 root         (0) root         (0)      160 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/pip/pip.conf.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.877155 adaux-2.2.0/source/adaux/src/pre-commit/
+-rwxrwxrwx   0 root         (0) root         (0)     1680 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/pre-commit/add_copy_right.py.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     5098 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/pre-commit/config.yaml.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)       84 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/pre-commit/mypy.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.881155 adaux-2.2.0/source/adaux/src/root/
+-rw-rw-rw-   0 root         (0) root         (0)      144 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/root/_setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      146 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/root/gitignore.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      487 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/root/setup.cfg.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.881155 adaux-2.2.0/source/adaux/src/root/source/
+-rw-rw-rw-   0 root         (0) root         (0)      126 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/root/source/gitignore.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      127 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/temp-combination
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.813153 adaux-2.2.0/source/adaux.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      314 2023-04-11 12:41:58.000000 adaux-2.2.0/source/adaux.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5236 2023-04-11 12:41:58.000000 adaux-2.2.0/source/adaux.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 12:41:58.000000 adaux-2.2.0/source/adaux.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-04-11 12:41:58.000000 adaux-2.2.0/source/adaux.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 12:40:53.000000 adaux-2.2.0/source/adaux.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      203 2023-04-11 12:41:58.000000 adaux-2.2.0/source/adaux.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-04-11 12:41:58.000000 adaux-2.2.0/source/adaux.egg-info/top_level.txt
```

### Comparing `adaux-2.1.1/LICENSE.txt` & `adaux-2.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `adaux-2.1.1/setup.cfg` & `adaux-2.2.0/setup.cfg`

 * *Files 26% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 test = 
 	pytest>=7.2
 	pytest-cov~=4.0
 
 [tool:pytest]
 markers = 
 	merge_only: run test only on merge request
-addopts = --strict-markers -m "not merge_only"
-cache_dir = devops/cache/pytest
+	local: run local tests that need docker
+addopts = --strict-markers -m "not merge_only and not local"
+cache_dir = /Users/mskoenz/programming/hobby/administratum/auxilium/devops/cache/pytest
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `adaux-2.1.1/source/adaux/_base_parser.py` & `adaux-2.2.0/source/adaux/_base_parser.py`

 * *Files identical despite different names*

### Comparing `adaux-2.1.1/source/adaux/_cli.py` & `adaux-2.2.0/source/adaux/_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -366,20 +366,23 @@
 
 @adaux.command()
 @click.pass_context
 @click.argument("payload_names", nargs=-1)
 @click.option(
     "-f", "--force", is_flag=True, default=False, help="runs payload even if up to date"
 )
-def run(ctx: click.Context, payload_names: tp.Tuple[str, ...], force: bool) -> None:
+@click.option("-d", "--dry", is_flag=True, default=False)
+def run(
+    ctx: click.Context, payload_names: tp.Tuple[str, ...], force: bool, dry: bool
+) -> None:
     """
     Run a specified payload. Use 'ls' to list all available payloads.
     """
     with convert_runtime_to_click_error():
-        ctx.obj.run(*payload_names, force=force)
+        ctx.obj.run(*payload_names, force=force, dry=dry)
 
 
 @adaux.command()
 @click.pass_context
 @click.option("-h", "--open-html", is_flag=True, default=False)
 def docs(ctx: click.Context, open_html: bool) -> None:
     """
@@ -494,15 +497,15 @@
     try:
         yield
     except RuntimeError as err:
         raise click.UsageError(err.args[0])
 
 
 def raise_if_not_init(ctx: click.Context) -> None:
-    if ctx.invoked_subcommand not in ["init"]:
+    if ctx.invoked_subcommand not in ["init", "demo"]:
         raise click.UsageError(
             f"{ctx.obj.auxcon_file} does not exists! use 'adaux init' to create one."
         )
 
 
 def raise_if_init_and_not_force(ctx: click.Context) -> None:
     if ctx.invoked_subcommand in ["init"]:
```

### Comparing `adaux-2.1.1/source/adaux/_cli_mixin.py` & `adaux-2.2.0/source/adaux/_cli_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,15 +218,17 @@
         cmd = [
             "sh",
             str(self.target / "docker" / f"{composition}-compose.sh"),
             *args,
         ]
         subprocess.run(cmd, check=False)
 
-    def run(self: "CliMixin", *payload_names: str, force: bool = False) -> None:
+    def run(
+        self: "CliMixin", *payload_names: str, force: bool = False, dry: bool = False
+    ) -> None:
         self._raise_if_disabled("payload")
         with self.extra(ExtraLevel.HYDRATED), self.cwd_to_root():
             data = self.auxh.payload
             if payload_names == ("ls",):
                 for title, flavor in [
                     ("payloads", "docker_build"),
                     ("with deps", "with_dependency"),
@@ -243,15 +245,15 @@
                 return
             try:
                 payloads = [data.lookup[x] for x in payload_names]
             except KeyError as err:
                 raise RuntimeError(
                     f"payload '{payload_names}' not found! Use aux run ls, or check the {self.auxcon_file.name} file."
                 ) from err
-            success = self.payload_run(*payloads, force=force)  # type: ignore
+            success = self.payload_run(*payloads, force=force, dry=dry)  # type: ignore
             if not success:
                 sys.exit(1)
 
     def docs(self: "CliMixin", open_html: bool = False) -> None:
         self._raise_if_disabled("docs")
 
         docs_cache = self.target / "cache" / "docs"
```

### Comparing `adaux-2.1.1/source/adaux/_components/_01_file_io_support.py` & `adaux-2.2.0/source/adaux/_components/_01_file_io_support.py`

 * *Files identical despite different names*

### Comparing `adaux-2.1.1/source/adaux/_components/_02_base.py` & `adaux-2.2.0/source/adaux/_components/_02_base.py`

 * *Files identical despite different names*

### Comparing `adaux-2.1.1/source/adaux/_components/_03_meta.py` & `adaux-2.2.0/source/adaux/_components/_03_meta.py`

 * *Files identical despite different names*

### Comparing `adaux-2.1.1/source/adaux/_components/_04_monotonic_version.py` & `adaux-2.2.0/source/adaux/_components/_04_monotonic_version.py`

 * *Files identical despite different names*

### Comparing `adaux-2.1.1/source/adaux/_components/_05_project.py` & `adaux-2.2.0/source/adaux/_components/_05_project.py`

 * *Files identical despite different names*

### Comparing `adaux-2.1.1/source/adaux/_components/_06_dependency.py` & `adaux-2.2.0/source/adaux/_components/_06_dependency.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,15 @@
             elif mod in data and mod not in tpl.dependencies:
                 self._print(f"dependencies.{mod}: removed {data[mod]}", fg="red")
                 del data[mod]
 
         for mod in tpl.dependencies:
             if mod not in ["test", "docs", "dev"]:
                 continue
-            newer = {}
+            newer = {"adaux": self.parse_dep(self.versions.adaux)[1]}
             for dep in tpl.dependencies[mod]:
                 pkg, version = self.parse_dep(dep)
                 if version is not None:
                     newer[pkg] = version
 
             dep_list = data.get(mod, [])
             for i, dep in enumerate(dep_list):
@@ -90,14 +90,24 @@
                     arch, arch_pkgs = next(iter(pkg_or_map.items()))
                     if isinstance(arch_pkgs, str):
                         arch_pkgs = [arch_pkgs]
                     assert isinstance(arch_pkgs, tp.Sequence)
                     res[arch] = arch_pkgs
             data[key] = res
 
+        # warn if dev dependency is outdated
+        for pkg in data.dev:
+            if pkg.startswith("adaux"):
+                compare = self.auxe.versions.adaux
+                if pkg != compare:
+                    self._print(
+                        f"WARNING: your dev dependency {pkg} is different from installed {compare}, please fix.",
+                        fg="red",
+                    )
+
     @classmethod
     def parse_dep(cls, dep: str) -> tp.Tuple[str, tp.Optional[str]]:
         if "=" in dep:
             pkg, version = re.split("[=><~]{2}", dep, 1)
         else:
             pkg = dep
             version = None
```

### Comparing `adaux-2.1.1/source/adaux/_components/_07_package.py` & `adaux-2.2.0/source/adaux/_components/_07_package.py`

 * *Files identical despite different names*

### Comparing `adaux-2.1.1/source/adaux/_components/_08_pip.py` & `adaux-2.2.0/source/adaux/_components/_08_pip.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
         super().defaulted()
         self.auxd.setdefault("pip", _ProtoNamespace())
         for key in self.__keys():
             self.auxd.pip.setdefault(key, _ProtoNamespace())
 
     def demodata(self) -> None:
         super().demodata()
+        self.auxcon.setdefault("pip", _ProtoNamespace())
         data = self.auxcon.pip
         data.extra_index_url = _ProtoNamespace(
             demo="https://gitlab-ci-token:$CI_JOB_TOKEN@gitlab.x.y/api/v4/projects/118/packages/pypi/simple"
         )
         data.branch_match = _ProtoNamespace(
             demo=_ProtoNamespace(
                 url="https://gitlab-ci-token:$CI_JOB_TOKEN@gitlab.x.y/user/demo.git",
```

### Comparing `adaux-2.1.1/source/adaux/_components/_09_gitignore.py` & `adaux-2.2.0/source/adaux/_components/_09_gitignore.py`

 * *Files identical despite different names*

### Comparing `adaux-2.1.1/source/adaux/_components/_10_gitlab.py` & `adaux-2.2.0/source/adaux/_components/_10_gitlab.py`

 * *Files 4% similar despite different names*

```diff
@@ -94,7 +94,13 @@
                 val.setdefault(skey, sval)
 
         if "remote_user" in data and "remote_url" in data:
             remote_name = data.get("remote_name", self.auxe.project.second_name)
             self.auxe.project.project_urls.Source = (
                 f"https://{data.remote_url}/{data.remote_user}/{remote_name}"
             )
+
+        proc = subprocess.run(
+            ["git", "branch", "--show-current"], capture_output=True, check=False
+        )
+        if proc.returncode == 0:
+            data.setdefault("current_branch", proc.stdout.decode("utf-8").strip())
```

### Comparing `adaux-2.1.1/source/adaux/_components/_11_precommit.py` & `adaux-2.2.0/source/adaux/_components/_11_precommit.py`

 * *Files identical despite different names*

### Comparing `adaux-2.1.1/source/adaux/_components/_12_pylint.py` & `adaux-2.2.0/source/adaux/_components/_12_pylint.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     def __keys(cls) -> tp.Tuple[str, ...]:
         return (
             "disable",
             "good_names",
             "class_attr_rgx",
             "min_similarity_lines",
             "argument_rgx",
+            "attr_rgx",
             "function_rgx",
             "variable_rgx",
             "method_rgx",
         )
 
     def templated(self) -> None:
         super().templated()
@@ -109,14 +110,15 @@
                 ("BASIC", "good-names", "good_names"),
                 ("SIMILARITIES", "min-similarity-lines", "min_similarity_lines"),
                 ("BASIC", "variable-rgx", "variable_rgx"),
                 ("BASIC", "const-rgx", "const_rgx"),
                 ("BASIC", "function-rgx", "function_rgx"),
                 ("BASIC", "argument-rgx", "argument_rgx"),
                 ("BASIC", "class-rgx", "class_rgx"),
+                ("BASIC", "attr-rgx", "attr_rgx"),
                 ("BASIC", "method-rgx", "method_rgx"),
                 ("BASIC", "attr-rgx", "attr_rgx"),
                 ("BASIC", "class-attribute-rgx", "class_attr_rgx"),
             ]:
                 subconfig = config[key1]
                 data = self.auxe[key]
                 if key2 in ["good-names", "disable"]:
```

### Comparing `adaux-2.1.1/source/adaux/_components/_13_executable.py` & `adaux-2.2.0/source/adaux/_components/_13_executable.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,14 +22,15 @@
         super().defaulted()
         self.auxd.setdefault("executables", _ProtoNamespace())
         for key in self.__keys():
             self.auxd.executables.setdefault(key, [])
 
     def demodata(self) -> None:
         super().demodata()
+        self.auxcon.setdefault("executables", _ProtoNamespace())
         data = self.auxcon.executables
         data.scripts = ["scripts/say_hello"]
 
     def bake(self) -> None:
         super().bake()
         config = self.auxe.project.config
         data = self.auxe.executables
```

### Comparing `adaux-2.1.1/source/adaux/_components/_14_mypy.py` & `adaux-2.2.0/source/adaux/_components/_14_mypy.py`

 * *Files identical despite different names*

### Comparing `adaux-2.1.1/source/adaux/_components/_15_pytest.py` & `adaux-2.2.0/source/adaux/_components/_15_pytest.py`

 * *Files identical despite different names*

### Comparing `adaux-2.1.1/source/adaux/_components/_17_docs.py` & `adaux-2.2.0/source/adaux/_components/_17_docs.py`

 * *Files identical despite different names*

### Comparing `adaux-2.1.1/source/adaux/_components/_18_payload.py` & `adaux-2.2.0/source/adaux/_components/_18_payload.py`

 * *Files 1% similar despite different names*

```diff
@@ -301,16 +301,21 @@
                 return self.payload.is_up_to_date()
 
             def script(self) -> None:
                 self.payload.run(self.force)
 
             def is_included(self, env: tp.Mapping[str, tp.Any]) -> tp.Tuple[bool, str]:
                 if isinstance(self.payload, DockerBuildPayload):
-                    if self.payload.is_up_to_date() and not self.force:
+                    res = self.is_up_to_date(env)
+                    if res:
                         return False, f"{self.payload.executor.tag} exists"
+                    if self.payload.param.get("always_build", False):
+                        return True, "always_build=True"
+                    if self.force:
+                        return True, "--force"
                     return True, f"missing {self.payload.executor.tag}"
 
                 return super().is_included(env)
 
         jman = JobManager(env=dict(verbose=True))
 
         def demo(*pld: Payload) -> tp.List[PayloadJob]:
```

### Comparing `adaux-2.1.1/source/adaux/_components/_19_docker.py` & `adaux-2.2.0/source/adaux/_components/_19_docker.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,17 @@
             data.docker_run["gitlab-release-run"] = _ProtoNamespace()
             data.python["gitlab-release"] = _ProtoNamespace()
             data.docker_run["pkg-gitlab"] = _ProtoNamespace()
 
     def demodata(self) -> None:
         super().demodata()
         data = self.auxcon.payload
-        data.docker_settings = _ProtoNamespace(platform="amd64")
+        data.docker_settings = _ProtoNamespace(
+            platform="amd64", base_match={"mybase": dict(fallback="develop")}
+        )
 
     def update_to_template(self, tpl: _ProtoNamespace, full: _ProtoNamespace) -> None:
         super().update_to_template(tpl, full)
 
         for flavor in ["docker_build", "docker_run", "with_dependency"]:
             if flavor not in self.auxf.payload:
                 continue
```

### Comparing `adaux-2.1.1/source/adaux/_components/_20_ci.py` & `adaux-2.2.0/source/adaux/_components/_20_ci.py`

 * *Files identical despite different names*

### Comparing `adaux-2.1.1/source/adaux/_components/_98_sentinel.py` & `adaux-2.2.0/source/adaux/_components/_98_sentinel.py`

 * *Files identical despite different names*

### Comparing `adaux-2.1.1/source/adaux/_components/_99_all.py` & `adaux-2.2.0/source/adaux/_components/_99_all.py`

 * *Files identical despite different names*

### Comparing `adaux-2.1.1/source/adaux/_components/_aux_ci.py` & `adaux-2.2.0/source/adaux/_components/_aux_ci.py`

 * *Files identical despite different names*

### Comparing `adaux-2.1.1/source/adaux/_components/_payload/__init__.py` & `adaux-2.2.0/source/adaux/_components/_payload/__init__.py`

 * *Files identical despite different names*

### Comparing `adaux-2.1.1/source/adaux/_components/_payload/_base.py` & `adaux-2.2.0/source/adaux/_components/_payload/_base.py`

 * *Files identical despite different names*

### Comparing `adaux-2.1.1/source/adaux/_components/_payload/_docker.py` & `adaux-2.2.0/source/adaux/_components/_payload/_docker.py`

 * *Files identical despite different names*

### Comparing `adaux-2.1.1/source/adaux/_components/_payload/_docker_build.py` & `adaux-2.2.0/source/adaux/_components/_payload/_docker_build.py`

 * *Files 27% similar despite different names*

```diff
@@ -11,19 +11,26 @@
 
 
 @dc.dataclass
 class DockerBuildPayload(DockerPayload):
     flavor: tp.ClassVar[str] = "docker_build"
 
     def create_executor(self, parents: tp.Any) -> tp.Any:
+        images = []
+        base = self.param.get("base")
+        if base:
+            images.append(base)
         return DockerBuild(
+            images=images,
             slug=self.auxh.project.slug,
             service=self.param.service_name,
             image_name=self.param.image_name,
-            branch_match=[],
-            base_match=[],
+            branch_match=self.param.get("branch_match", []),
+            base_match=self.param.get("base_match", []),
             parents=parents,
             files=[f"devops/docker/{self.param.service_name}.dockerfile"],
         )
 
     def is_up_to_date(self) -> bool:
+        if self.param.get("always_build", False):
+            return False
         return self.executor.is_up_to_date()  # type: ignore
```

### Comparing `adaux-2.1.1/source/adaux/_components/_payload/_docker_executors.py` & `adaux-2.2.0/source/adaux/_components/_payload/_docker_executors.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,22 @@
 
     # Run local registry:
     # docker run -d -p 5000:5000 --name registry registry:2
     # docker container stop registry && docker container rm -v registry
     # export CI_REGISTRY=localhost:5000
     @property
     def registry_host(self) -> str:
+        if not self.remote_exists():
+            raise RuntimeError(
+                "Your run needs a remote registry.\n"
+                "In case you have not already, you can launch a local registry with\n"
+                "  docker run -d -p 5000:5000 --name registry registry:2\n"
+                "and run\n"
+                "  export CI_REGISTRY=localhost:5000"
+            )
         return os.environ["CI_REGISTRY"]
 
     def remote_exists(self) -> bool:
         return "CI_REGISTRY" in os.environ
 
     @property
     def build_deps(self) -> tp.Iterator["DockerBuildMixin"]:
```

### Comparing `adaux-2.1.1/source/adaux/_components/_payload/_python.py` & `adaux-2.2.0/source/adaux/_components/_payload/_python.py`

 * *Files identical despite different names*

### Comparing `adaux-2.1.1/source/adaux/_components/_payload/_with_dependency.py` & `adaux-2.2.0/source/adaux/_components/_payload/_with_dependency.py`

 * *Files identical despite different names*

### Comparing `adaux-2.1.1/source/adaux/_create_badge.py` & `adaux-2.2.0/source/adaux/_create_badge.py`

 * *Files identical despite different names*

### Comparing `adaux-2.1.1/source/adaux/_gitlab.py` & `adaux-2.2.0/source/adaux/_gitlab.py`

 * *Files 3% similar despite different names*

```diff
@@ -202,27 +202,31 @@
 
     def bake(self) -> None:
         self.sync_settings()
         self.sync_badges()
         self.sync_protection()
 
     @staticmethod
-    def _col(x: tp.Any) -> str:
+    def _col(x: tp.Any) -> tp.Union[str, tp.Tuple[int, int, int]]:
         status = x["status"]
+        col: tp.Union[str, tp.Tuple[int, int, int]] = "yellow"
         if status == "success":
-            return "green"
-        if status == "failed":
-            return "red"
-        if status == "pending":
-            return "blue"
-        if status == "created":
-            return "cyan"
-        if status == "canceled":
-            return "magenta"
-        return "yellow"
+            col = "green"
+        elif status == "failed":
+            if x.get("allow_failure", False):
+                col = (191, 255, 0)  # lime
+            else:
+                col = "red"
+        elif status == "pending":
+            col = "blue"
+        elif status == "created":
+            col = "cyan"
+        elif status == "canceled":
+            col = "magenta"
+        return col
 
     def pipeline(self, show_success: bool = False) -> tp.Tuple[bool, bool]:
         out = subprocess.run(
             ["git", "rev-parse", "--abbrev-ref", "HEAD"],
             check=True,
             capture_output=True,
         )
```

### Comparing `adaux-2.1.1/source/adaux/_parser.py` & `adaux-2.2.0/source/adaux/_parser.py`

 * *Files identical despite different names*

### Comparing `adaux-2.1.1/source/adaux/_proto_namespace.py` & `adaux-2.2.0/source/adaux/_proto_namespace.py`

 * *Files identical despite different names*

### Comparing `adaux-2.1.1/source/adaux/_tick.py` & `adaux-2.2.0/source/adaux/_tick.py`

 * *Files identical despite different names*

### Comparing `adaux-2.1.1/source/adaux/_todo.py` & `adaux-2.2.0/source/adaux/_todo.py`

 * *Files identical despite different names*

### Comparing `adaux-2.1.1/source/adaux/_util.py` & `adaux-2.2.0/source/adaux/_util.py`

 * *Files identical despite different names*

### Comparing `adaux-2.1.1/source/adaux/src/CI/00-main.yml.jinja2` & `adaux-2.2.0/source/adaux/src/CI/00-main.yml.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.1.1/source/adaux/src/CI/01-rules.yml.jinja2` & `adaux-2.2.0/source/adaux/src/CI/01-rules.yml.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.1.1/source/adaux/src/docker/services/ansible-deploy/Dockerfile.jinja2` & `adaux-2.2.0/source/adaux/src/docker/services/ansible-deploy/Dockerfile.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.1.1/source/adaux/src/docker/services/ansible-deploy/docker-compose.yml.jinja2` & `adaux-2.2.0/source/adaux/src/docker/services/ansible-deploy/docker-compose.yml.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.1.1/source/adaux/src/docker/services/docs/Dockerfile.jinja2` & `adaux-2.2.0/source/adaux/src/docker/services/docs/Dockerfile.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.1.1/source/adaux/src/docker/services/gitlab-release-run/docker-compose.yml.jinja2` & `adaux-2.2.0/source/adaux/src/docker/services/gitlab-release-run/docker-compose.yml.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.1.1/source/adaux/src/docker/services/image/Dockerfile.jinja2` & `adaux-2.2.0/source/adaux/src/docker/services/image/Dockerfile.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.1.1/source/adaux/src/docker/services/image-pytest/Dockerfile.jinja2` & `adaux-2.2.0/source/adaux/src/docker/services/image-pytest/Dockerfile.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.1.1/source/adaux/src/docker/services/jinja-snippets/docker-build.jinja2` & `adaux-2.2.0/source/adaux/src/docker/services/jinja-snippets/docker-build.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.1.1/source/adaux/src/docker/services/pkg-gitlab/docker-compose.yml.jinja2` & `adaux-2.2.0/source/adaux/src/docker/services/pkg-gitlab/docker-compose.yml.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.1.1/source/adaux/src/docker/services/pre-commit/Dockerfile.jinja2` & `adaux-2.2.0/source/adaux/src/docker/services/pre-commit/Dockerfile.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.1.1/source/adaux/src/docker/services/pre-commit/docker-compose.yml.jinja2` & `adaux-2.2.0/source/adaux/src/docker/services/pre-commit/docker-compose.yml.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.1.1/source/adaux/src/docker/services/pytest-standalone/Dockerfile.jinja2` & `adaux-2.2.0/source/adaux/src/docker/services/pytest-standalone/Dockerfile.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.1.1/source/adaux/src/docker/services/python-deps/Dockerfile.jinja2` & `adaux-2.2.0/source/adaux/src/docker/services/python-deps/Dockerfile.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.1.1/source/adaux/src/docs/default_conf.py.jinja2` & `adaux-2.2.0/source/adaux/src/docs/default_conf.py.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.1.1/source/adaux/src/docs/postprocess_html.py` & `adaux-2.2.0/source/adaux/src/docs/postprocess_html.py`

 * *Files identical despite different names*

### Comparing `adaux-2.1.1/source/adaux/src/license/Apache-2.0.txt.jinja2` & `adaux-2.2.0/source/adaux/src/license/Apache-2.0.txt.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.1.1/source/adaux/src/license/BSD-3_clause.txt.jinja2` & `adaux-2.2.0/source/adaux/src/license/BSD-3_clause.txt.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.1.1/source/adaux/src/license/MIT.txt.jinja2` & `adaux-2.2.0/source/adaux/src/license/MIT.txt.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.1.1/source/adaux/src/payload/python/__pycache__/functions.cpython-310.pyc` & `adaux-2.2.0/source/adaux/src/payload/python/__pycache__/functions.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr  4 14:24:52 2023 UTC, .py size: 2816 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 19% similar despite different names*

```diff
@@ -1,152 +1,163 @@
-00000000: 6f0d 0d0a 0000 0000 3433 2c64 000b 0000  o.......43,d....
+00000000: 6f0d 0d0a 0000 0000 3872 3464 2d0c 0000  o.......8r4d-...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0008 0000 0040 0000 0073 a800 0000 6400  .....@...s....d.
+00000020: 0009 0000 0040 0000 0073 b800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a03 6402 6403 6c04 6d05 5a05  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6402 6404 6c04 6d06 5a06 0100 6402  ..d.d.l.m.Z...d.
 00000060: 6405 6c04 6d07 5a07 0100 6402 6406 6c08  d.l.m.Z...d.d.l.
 00000070: 6d09 5a09 0100 6407 6509 6408 6401 6604  m.Z...d.e.d.d.f.
 00000080: 6409 640a 8404 5a0a 6407 6509 6408 6401  d.d...Z.d.e.d.d.
 00000090: 6604 640b 640c 8404 5a0b 6407 6509 640d  f.d.d...Z.d.e.d.
-000000a0: 6503 6a0c 640e 650d 6408 6401 6608 640f  e.j.d.e.d.d.f.d.
-000000b0: 640e 8404 5a0e 6407 6509 640d 6503 6a0c  d...Z.d.e.d.e.j.
-000000c0: 6410 650d 6408 6401 6608 6411 6412 8404  d.e.d.d.f.d.d...
-000000d0: 5a0f 6401 5300 2913 e900 0000 004e e904  Z.d.S.)......N..
-000000e0: 0000 0029 01da 0e73 7562 7072 6f63 6573  ...)...subproces
-000000f0: 735f 7275 6e29 01da 0974 6167 5f69 6d61  s_run)...tag_ima
-00000100: 6765 2901 da10 7570 6c6f 6164 5f74 6f5f  ge)...upload_to_
-00000110: 7265 6d6f 7465 2901 da0f 5f50 726f 746f  remote)..._Proto
-00000120: 4e61 6d65 7370 6163 65da 0361 7578 da06  Namespace..aux..
-00000130: 7265 7475 726e 6301 0000 0000 0000 0000  returnc.........
-00000140: 0000 0005 0000 0006 0000 0043 0000 0073  ...........C...s
-00000150: 8600 0000 7c00 6a00 6a01 7d01 7c00 6a00  ....|.j.j.}.|.j.
-00000160: 6a02 7d02 7c02 7c01 7601 7214 7403 6401  j.}.|.|.v.r.t.d.
-00000170: 7c02 9b00 6402 9d03 8301 8201 7404 6700  |...d.......t.g.
-00000180: 6403 a201 6404 6404 6405 8d03 7d03 7405  d...d.d.d...}.t.
-00000190: 7406 a007 6406 7c03 6a08 a009 a100 a102  t...d.|.j.......
-000001a0: 8301 7d04 7c02 7c04 7600 7234 7403 6401  ..}.|.|.v.r4t.d.
-000001b0: 7c02 9b00 6407 9d03 8301 8201 740a 6401  |...d.......t.d.
-000001c0: 7c02 9b00 6408 7c01 7c02 1900 9b00 6409  |...d.|.|.....d.
-000001d0: 9d05 8301 0100 6400 5300 290a 4e7a 0876  ......d.S.).Nz.v
-000001e0: 6572 7369 6f6e 207a 2520 6973 206e 6f74  ersion z% is not
-000001f0: 2069 6e20 7265 6c65 6173 6520 6e6f 7465   in release note
-00000200: 732c 2070 6c65 6173 6520 6164 6421 2903  s, please add!).
-00000210: da03 6769 747a 096c 732d 7265 6d6f 7465  ..gitz.ls-remote
-00000220: 7a06 2d2d 7461 6773 5429 02da 0563 6865  z.--tagsT)...che
-00000230: 636b da0e 6361 7074 7572 655f 6f75 7470  ck..capture_outp
-00000240: 7574 7a0f 7461 6773 2f28 5b5c 642e 5d2b  utz.tags/([\d.]+
-00000250: 295c 6e7a 3320 7761 7320 616c 7265 6164  )\nz3 was alread
-00000260: 7920 7265 6c65 6173 6564 2061 6e64 2063  y released and c
-00000270: 616e 6e6f 7420 6265 2072 656c 6561 7365  annot be release
-00000280: 6420 6167 6169 6e21 7a12 2068 6173 2064  d again!z. has d
-00000290: 6573 6372 6970 7469 6f6e 2027 fa01 2729  escription '..')
-000002a0: 0bda 0770 726f 6a65 6374 da0d 7265 6c65  ...project..rele
-000002b0: 6173 655f 6e6f 7465 73da 0776 6572 7369  ase_notes..versi
-000002c0: 6f6e da0c 5275 6e74 696d 6545 7272 6f72  on..RuntimeError
-000002d0: 7203 0000 00da 046c 6973 74da 0272 65da  r......list..re.
-000002e0: 0766 696e 6461 6c6c da06 7374 646f 7574  .findall..stdout
-000002f0: da06 6465 636f 6465 da05 7072 696e 7429  ..decode..print)
-00000300: 0572 0700 0000 720e 0000 0072 0f00 0000  .r....r....r....
-00000310: da03 6f75 745a 1061 6c72 6561 6479 5f72  ..outZ.already_r
-00000320: 656c 6561 7365 64a9 0072 1800 0000 fa39  eleased..r.....9
-00000330: 2f62 7569 6c64 732f 726f 6f74 2f73 6f75  /builds/root/sou
-00000340: 7263 652f 6164 6175 782f 7372 632f 7061  rce/adaux/src/pa
-00000350: 796c 6f61 642f 7079 7468 6f6e 2f66 756e  yload/python/fun
-00000360: 6374 696f 6e73 2e70 79da 1363 6865 636b  ctions.py..check
-00000370: 5f72 656c 6561 7365 5f6e 6f74 6573 0c00  _release_notes..
-00000380: 0000 731a 0000 0008 0108 0108 0210 0102  ..s.............
-00000390: 020a 0106 ff16 0308 0102 010a 0104 ff1e  ................
-000003a0: 0472 1a00 0000 6301 0000 0000 0000 0000  .r....c.........
-000003b0: 0000 0005 0000 0003 0000 0043 0000 0073  ...........C...s
-000003c0: 4400 0000 7c00 6a00 6a01 7d01 7c00 6a00  D...|.j.j.}.|.j.
-000003d0: 6a02 7d02 7c01 7c02 1900 7d03 7c02 7403  j.}.|.|...}.|.t.
-000003e0: 6a04 6401 3c00 7c03 7403 6a04 6402 3c00  j.d.<.|.t.j.d.<.
-000003f0: 7c00 6a05 6a06 6403 1900 7d04 7c04 a007  |.j.j.d...}.|...
-00000400: a100 0100 6400 5300 2904 4e5a 0b52 454c  ....d.S.).NZ.REL
-00000410: 4541 5345 5f54 4147 5a13 5245 4c45 4153  EASE_TAGZ.RELEAS
-00000420: 455f 4445 5343 5249 5054 494f 4e7a 1267  E_DESCRIPTIONz.g
-00000430: 6974 6c61 622d 7265 6c65 6173 652d 7275  itlab-release-ru
-00000440: 6e29 0872 0d00 0000 720e 0000 0072 0f00  n).r....r....r..
-00000450: 0000 da02 6f73 da07 656e 7669 726f 6eda  ....os..environ.
-00000460: 0770 6179 6c6f 6164 da06 6c6f 6f6b 7570  .payload..lookup
-00000470: da03 7275 6e29 0572 0700 0000 720e 0000  ..run).r....r...
-00000480: 0072 0f00 0000 da0b 6465 7363 7269 7074  .r......descript
-00000490: 696f 6e72 1d00 0000 7218 0000 0072 1800  ionr....r....r..
-000004a0: 0000 7219 0000 00da 0e67 6974 6c61 625f  ..r......gitlab_
-000004b0: 7265 6c65 6173 651f 0000 0073 0e00 0000  release....s....
-000004c0: 0801 0801 0801 0a01 0a01 0c01 0c01 7221  ..............r!
-000004d0: 0000 00da 0464 6570 73da 0374 6167 6303  .....deps..tagc.
-000004e0: 0000 0000 0000 0000 0000 0005 0000 0006  ................
-000004f0: 0000 0043 0000 0073 6200 0000 7400 7c01  ...C...sb...t.|.
-00000500: 8301 6401 6b03 7213 7401 6402 7c02 9b00  ..d.k.r.t.d.|...
-00000510: 6403 7400 7c01 8301 9b00 6404 9d05 8301  d.t.|.....d.....
-00000520: 8201 7c02 6a02 7c00 6a03 6a04 6405 8d01  ..|.j.|.j.j.d...
-00000530: 7d02 7c01 6406 1900 6a05 a006 7c02 a101  }.|.d...j...|...
-00000540: 5c02 7d03 7d04 7407 6407 7c03 8302 0100  \.}.}.t.d.|.....
-00000550: 7407 6408 7c04 8302 0100 6400 5300 2909  t.d.|.....d.S.).
-00000560: 4ee9 0100 0000 7a0c 7461 6720 6a6f 6220  N.....z.tag job 
-00000570: 666f 7220 fa27 2073 686f 756c 6420 6861  for .' should ha
-00000580: 7665 2065 7861 6374 6c79 2031 2064 6570  ve exactly 1 dep
-00000590: 656e 6465 6e63 792c 206e 6f74 20fa 0121  endency, not ..!
-000005a0: 2901 720f 0000 0072 0100 0000 da08 7570  ).r....r......up
-000005b0: 6c6f 6164 6564 fa08 2020 202d 3e20 746f  loaded..   -> to
-000005c0: 2908 da03 6c65 6e72 1000 0000 da06 666f  )...lenr......fo
-000005d0: 726d 6174 720d 0000 0072 0f00 0000 da08  rmatr....r......
-000005e0: 6578 6563 7574 6f72 da0e 7461 675f 616e  executor..tag_an
-000005f0: 645f 7570 6c6f 6164 7216 0000 0029 0572  d_uploadr....).r
-00000600: 0700 0000 7222 0000 0072 2300 0000 da09  ....r"...r#.....
-00000610: 6c6f 6361 6c5f 7461 67da 0b72 656c 6561  local_tag..relea
-00000620: 7365 5f74 6167 7218 0000 0072 1800 0000  se_tagr....r....
-00000630: 7219 0000 0072 2300 0000 2900 0000 7310  r....r#...)...s.
-00000640: 0000 000c 0502 0114 0104 ff10 0314 010a  ................
-00000650: 010e 0172 2e00 0000 6303 0000 0000 0000  ...r....c.......
-00000660: 0000 0000 0004 0000 0008 0000 0043 0000  .............C..
-00000670: 0073 a400 0000 7400 7c01 8301 6401 6b03  .s....t.|...d.k.
-00000680: 7213 7401 6402 7c02 9b00 6403 7400 7c01  r.t.d.|...d.t.|.
-00000690: 8301 9b00 6404 9d05 8301 8201 7c02 6a02  ....d.......|.j.
-000006a0: 7c00 6a03 6a04 7c00 6a05 6a06 6405 8d02  |.j.j.|.j.j.d...
-000006b0: 7d02 7c01 6406 1900 6a07 a008 a100 7d03  }.|.d...j.....}.
-000006c0: 7409 7c03 7c02 8302 0100 740a 6407 6408  t.|.|.....t.d.d.
-000006d0: 6409 740b 6a0c 640a 1900 640b 740b 6a0c  d.t.j.d...d.t.j.
-000006e0: 640c 1900 640d 6707 8301 0100 740d 7c03  d...d.g.....t.|.
-000006f0: 7c02 8302 0100 740a 6700 640e a201 8301  |.....t.g.d.....
-00000700: 0100 740e 640f 7c03 8302 0100 740e 6410  ..t.d.|.....t.d.
-00000710: 7c02 8302 0100 6400 5300 2911 4e72 2400  |.....d.S.).Nr$.
-00000720: 0000 7a16 696d 672d 646f 636b 6572 6875  ..z.img-dockerhu
-00000730: 6220 6a6f 6220 666f 7220 7225 0000 0072  b job for r%...r
-00000740: 2600 0000 2902 720f 0000 00da 0e63 695f  &...).r......ci_
-00000750: 6164 6175 785f 696d 6167 6572 0100 0000  adaux_imager....
-00000760: da06 646f 636b 6572 da05 6c6f 6769 6e7a  ..docker..loginz
-00000770: 022d 755a 1244 4f43 4b45 5248 5542 5f55  .-uZ.DOCKERHUB_U
-00000780: 5345 524e 414d 457a 022d 705a 1244 4f43  SERNAMEz.-pZ.DOC
-00000790: 4b45 5248 5542 5f50 4153 5357 4f52 44fa  KERHUB_PASSWORD.
-000007a0: 0964 6f63 6b65 722e 696f 2903 7230 0000  .docker.io).r0..
-000007b0: 005a 066c 6f67 6f75 7472 3200 0000 7227  .Z.logoutr2...r'
-000007c0: 0000 0072 2800 0000 290f 7229 0000 0072  ...r(...).r)...r
-000007d0: 1000 0000 722a 0000 0072 0d00 0000 720f  ....r*...r....r.
-000007e0: 0000 00da 0876 6572 7369 6f6e 7372 2f00  .....versionsr/.
-000007f0: 0000 722b 0000 00da 1470 756c 6c5f 6966  ..r+.....pull_if
-00000800: 5f6e 6f74 5f65 7869 7374 656e 7472 0400  _not_existentr..
-00000810: 0000 7203 0000 0072 1b00 0000 721c 0000  ..r....r....r...
-00000820: 0072 0500 0000 7216 0000 0029 0472 0700  .r....r....).r..
-00000830: 0000 7222 0000 0072 2e00 0000 722d 0000  ..r"...r....r-..
-00000840: 0072 1800 0000 7218 0000 0072 1900 0000  .r....r....r....
-00000850: da0d 696d 675f 646f 636b 6572 6875 6238  ..img_dockerhub8
-00000860: 0000 0073 2e00 0000 0c05 0201 1401 04ff  ...s............
-00000870: 0403 0c01 06ff 0e03 0a01 0201 0202 0201  ................
-00000880: 0201 0801 0201 0801 0201 02f9 04ff 0a0b  ................
-00000890: 0c01 0a01 0e01 7235 0000 0029 1072 1b00  ......r5...).r..
-000008a0: 0000 7212 0000 00da 0674 7970 696e 67da  ..r......typing.
-000008b0: 0274 705a 265f 636f 6d70 6f6e 656e 7473  .tpZ&_components
-000008c0: 2e5f 7061 796c 6f61 642e 5f64 6f63 6b65  ._payload._docke
-000008d0: 725f 6578 6563 7574 6f72 7372 0300 0000  r_executorsr....
-000008e0: 7204 0000 0072 0500 0000 da10 5f70 726f  r....r......_pro
-000008f0: 746f 5f6e 616d 6573 7061 6365 7206 0000  to_namespacer...
-00000900: 0072 1a00 0000 7221 0000 00da 0341 6e79  .r....r!.....Any
-00000910: da03 7374 7272 2300 0000 7235 0000 0072  ..strr#...r5...r
-00000920: 1800 0000 7218 0000 0072 1800 0000 7219  ....r....r....r.
-00000930: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-00000940: 0073 3600 0000 0801 0801 0801 0c02 0c01  .s6.............
-00000950: 0c01 0c01 1203 1213 020a 0201 02ff 0402  ................
-00000960: 02fe 0203 02fd 0204 0afc 020f 0201 02ff  ................
-00000970: 0402 02fe 0203 02fd 0204 0efc            ............
+000000a0: 6503 6a0c 640e 6503 6a0d 650e 6503 6a0f  e.j.d.e.j.e.e.j.
+000000b0: 650e 1900 6602 1900 6408 6401 6608 640f  e...f...d.d.f.d.
+000000c0: 6410 8404 5a10 6407 6509 640d 6503 6a0c  d...Z.d.e.d.e.j.
+000000d0: 6411 650e 6408 6401 6608 6412 6413 8404  d.e.d.d.f.d.d...
+000000e0: 5a11 6401 5300 2914 e900 0000 004e e904  Z.d.S.)......N..
+000000f0: 0000 0029 01da 0e73 7562 7072 6f63 6573  ...)...subproces
+00000100: 735f 7275 6e29 01da 0974 6167 5f69 6d61  s_run)...tag_ima
+00000110: 6765 2901 da10 7570 6c6f 6164 5f74 6f5f  ge)...upload_to_
+00000120: 7265 6d6f 7465 2901 da0f 5f50 726f 746f  remote)..._Proto
+00000130: 4e61 6d65 7370 6163 65da 0361 7578 da06  Namespace..aux..
+00000140: 7265 7475 726e 6301 0000 0000 0000 0000  returnc.........
+00000150: 0000 0005 0000 0006 0000 0043 0000 0073  ...........C...s
+00000160: 8600 0000 7c00 6a00 6a01 7d01 7c00 6a00  ....|.j.j.}.|.j.
+00000170: 6a02 7d02 7c02 7c01 7601 7214 7403 6401  j.}.|.|.v.r.t.d.
+00000180: 7c02 9b00 6402 9d03 8301 8201 7404 6700  |...d.......t.g.
+00000190: 6403 a201 6404 6404 6405 8d03 7d03 7405  d...d.d.d...}.t.
+000001a0: 7406 a007 6406 7c03 6a08 a009 a100 a102  t...d.|.j.......
+000001b0: 8301 7d04 7c02 7c04 7600 7234 7403 6401  ..}.|.|.v.r4t.d.
+000001c0: 7c02 9b00 6407 9d03 8301 8201 740a 6401  |...d.......t.d.
+000001d0: 7c02 9b00 6408 7c01 7c02 1900 9b00 6409  |...d.|.|.....d.
+000001e0: 9d05 8301 0100 6400 5300 290a 4e7a 0876  ......d.S.).Nz.v
+000001f0: 6572 7369 6f6e 207a 2520 6973 206e 6f74  ersion z% is not
+00000200: 2069 6e20 7265 6c65 6173 6520 6e6f 7465   in release note
+00000210: 732c 2070 6c65 6173 6520 6164 6421 2903  s, please add!).
+00000220: da03 6769 747a 096c 732d 7265 6d6f 7465  ..gitz.ls-remote
+00000230: 7a06 2d2d 7461 6773 5429 02da 0563 6865  z.--tagsT)...che
+00000240: 636b da0e 6361 7074 7572 655f 6f75 7470  ck..capture_outp
+00000250: 7574 7a0f 7461 6773 2f28 5b5c 642e 5d2b  utz.tags/([\d.]+
+00000260: 295c 6e7a 3320 7761 7320 616c 7265 6164  )\nz3 was alread
+00000270: 7920 7265 6c65 6173 6564 2061 6e64 2063  y released and c
+00000280: 616e 6e6f 7420 6265 2072 656c 6561 7365  annot be release
+00000290: 6420 6167 6169 6e21 7a12 2068 6173 2064  d again!z. has d
+000002a0: 6573 6372 6970 7469 6f6e 2027 fa01 2729  escription '..')
+000002b0: 0bda 0770 726f 6a65 6374 da0d 7265 6c65  ...project..rele
+000002c0: 6173 655f 6e6f 7465 73da 0776 6572 7369  ase_notes..versi
+000002d0: 6f6e da0c 5275 6e74 696d 6545 7272 6f72  on..RuntimeError
+000002e0: 7203 0000 00da 046c 6973 74da 0272 65da  r......list..re.
+000002f0: 0766 696e 6461 6c6c da06 7374 646f 7574  .findall..stdout
+00000300: da06 6465 636f 6465 da05 7072 696e 7429  ..decode..print)
+00000310: 0572 0700 0000 720e 0000 0072 0f00 0000  .r....r....r....
+00000320: da03 6f75 745a 1061 6c72 6561 6479 5f72  ..outZ.already_r
+00000330: 656c 6561 7365 64a9 0072 1800 0000 fa39  eleased..r.....9
+00000340: 2f62 7569 6c64 732f 726f 6f74 2f73 6f75  /builds/root/sou
+00000350: 7263 652f 6164 6175 782f 7372 632f 7061  rce/adaux/src/pa
+00000360: 796c 6f61 642f 7079 7468 6f6e 2f66 756e  yload/python/fun
+00000370: 6374 696f 6e73 2e70 79da 1363 6865 636b  ctions.py..check
+00000380: 5f72 656c 6561 7365 5f6e 6f74 6573 0c00  _release_notes..
+00000390: 0000 731a 0000 0008 0108 0108 0210 0102  ..s.............
+000003a0: 020a 0106 ff16 0308 0102 010a 0104 ff1e  ................
+000003b0: 0472 1a00 0000 6301 0000 0000 0000 0000  .r....c.........
+000003c0: 0000 0005 0000 0003 0000 0043 0000 0073  ...........C...s
+000003d0: 4400 0000 7c00 6a00 6a01 7d01 7c00 6a00  D...|.j.j.}.|.j.
+000003e0: 6a02 7d02 7c01 7c02 1900 7d03 7c02 7403  j.}.|.|...}.|.t.
+000003f0: 6a04 6401 3c00 7c03 7403 6a04 6402 3c00  j.d.<.|.t.j.d.<.
+00000400: 7c00 6a05 6a06 6403 1900 7d04 7c04 a007  |.j.j.d...}.|...
+00000410: a100 0100 6400 5300 2904 4e5a 0b52 454c  ....d.S.).NZ.REL
+00000420: 4541 5345 5f54 4147 5a13 5245 4c45 4153  EASE_TAGZ.RELEAS
+00000430: 455f 4445 5343 5249 5054 494f 4e7a 1267  E_DESCRIPTIONz.g
+00000440: 6974 6c61 622d 7265 6c65 6173 652d 7275  itlab-release-ru
+00000450: 6e29 0872 0d00 0000 720e 0000 0072 0f00  n).r....r....r..
+00000460: 0000 da02 6f73 da07 656e 7669 726f 6eda  ....os..environ.
+00000470: 0770 6179 6c6f 6164 da06 6c6f 6f6b 7570  .payload..lookup
+00000480: da03 7275 6e29 0572 0700 0000 720e 0000  ..run).r....r...
+00000490: 0072 0f00 0000 da0b 6465 7363 7269 7074  .r......descript
+000004a0: 696f 6e72 1d00 0000 7218 0000 0072 1800  ionr....r....r..
+000004b0: 0000 7219 0000 00da 0e67 6974 6c61 625f  ..r......gitlab_
+000004c0: 7265 6c65 6173 651f 0000 0073 0e00 0000  release....s....
+000004d0: 0801 0801 0801 0a01 0a01 0c01 0c01 7221  ..............r!
+000004e0: 0000 00da 0464 6570 73da 0474 6167 7363  .....deps..tagsc
+000004f0: 0300 0000 0000 0000 0000 0000 0700 0000  ................
+00000500: 0600 0000 4300 0000 7392 0000 0074 007c  ....C...s....t.|
+00000510: 0274 0183 0272 087c 0267 017d 0274 027c  .t...r.|.g.}.t.|
+00000520: 0183 0164 016b 0372 1b74 0364 027c 029b  ...d.k.r.t.d.|..
+00000530: 0064 0374 027c 0183 019b 0064 049d 0583  .d.t.|.....d....
+00000540: 0182 0164 057d 037c 0244 005d 277d 047c  ...d.}.|.D.]'}.|
+00000550: 046a 047c 006a 056a 067c 006a 076a 0864  .j.|.j.j.|.j.j.d
+00000560: 068d 027d 047c 0164 0719 006a 09a0 0a7c  ...}.|.d...j...|
+00000570: 04a1 015c 027d 057d 067c 037c 056b 0372  ...\.}.}.|.|.k.r
+00000580: 417c 057d 0374 0b64 087c 0583 0201 0074  A|.}.t.d.|.....t
+00000590: 0b64 097c 0683 0201 0071 1f64 0053 0029  .d.|.....q.d.S.)
+000005a0: 0a4e e901 0000 007a 0c74 6167 206a 6f62  .N.....z.tag job
+000005b0: 2066 6f72 20fa 2720 7368 6f75 6c64 2068   for .' should h
+000005c0: 6176 6520 6578 6163 746c 7920 3120 6465  ave exactly 1 de
+000005d0: 7065 6e64 656e 6379 2c20 6e6f 7420 fa01  pendency, not ..
+000005e0: 21da 0029 0272 0f00 0000 da06 6272 616e  !..).r......bran
+000005f0: 6368 7201 0000 00da 0875 706c 6f61 6465  chr......uploade
+00000600: 64fa 0820 2020 2d3e 2074 6f29 0cda 0a69  d..   -> to)...i
+00000610: 7369 6e73 7461 6e63 65da 0373 7472 da03  sinstance..str..
+00000620: 6c65 6e72 1000 0000 da06 666f 726d 6174  lenr......format
+00000630: 720d 0000 0072 0f00 0000 da06 6769 746c  r....r......gitl
+00000640: 6162 da0e 6375 7272 656e 745f 6272 616e  ab..current_bran
+00000650: 6368 da08 6578 6563 7574 6f72 da0e 7461  ch..executor..ta
+00000660: 675f 616e 645f 7570 6c6f 6164 7216 0000  g_and_uploadr...
+00000670: 0029 0772 0700 0000 7222 0000 0072 2300  .).r....r"...r#.
+00000680: 0000 5a0e 6c61 7374 5f6c 6f63 616c 5f74  ..Z.last_local_t
+00000690: 6167 da03 7461 67da 096c 6f63 616c 5f74  ag..tag..local_t
+000006a0: 6167 da0b 7265 6c65 6173 655f 7461 6772  ag..release_tagr
+000006b0: 1800 0000 7218 0000 0072 1900 0000 7233  ....r....r....r3
+000006c0: 0000 0029 0000 0073 1e00 0000 0a05 0601  ...)...s........
+000006d0: 0c02 0201 1401 04ff 0403 0801 1601 1401  ................
+000006e0: 0801 0401 0a01 0c01 04fa 7233 0000 0072  ..........r3...r
+000006f0: 3500 0000 6303 0000 0000 0000 0000 0000  5...c...........
+00000700: 0004 0000 0008 0000 0043 0000 0073 a400  .........C...s..
+00000710: 0000 7400 7c01 8301 6401 6b03 7213 7401  ..t.|...d.k.r.t.
+00000720: 6402 7c02 9b00 6403 7400 7c01 8301 9b00  d.|...d.t.|.....
+00000730: 6404 9d05 8301 8201 7c02 6a02 7c00 6a03  d.......|.j.|.j.
+00000740: 6a04 7c00 6a05 6a06 6405 8d02 7d02 7c01  j.|.j.j.d...}.|.
+00000750: 6406 1900 6a07 a008 a100 7d03 7409 7c03  d...j.....}.t.|.
+00000760: 7c02 8302 0100 740a 6407 6408 6409 740b  |.....t.d.d.d.t.
+00000770: 6a0c 640a 1900 640b 740b 6a0c 640c 1900  j.d...d.t.j.d...
+00000780: 640d 6707 8301 0100 740d 7c03 7c02 8302  d.g.....t.|.|...
+00000790: 0100 740a 6700 640e a201 8301 0100 740e  ..t.g.d.......t.
+000007a0: 640f 7c03 8302 0100 740e 6410 7c02 8302  d.|.....t.d.|...
+000007b0: 0100 6400 5300 2911 4e72 2400 0000 7a16  ..d.S.).Nr$...z.
+000007c0: 696d 672d 646f 636b 6572 6875 6220 6a6f  img-dockerhub jo
+000007d0: 6220 666f 7220 7225 0000 0072 2600 0000  b for r%...r&...
+000007e0: 2902 720f 0000 00da 0e63 695f 6164 6175  ).r......ci_adau
+000007f0: 785f 696d 6167 6572 0100 0000 da06 646f  x_imager......do
+00000800: 636b 6572 da05 6c6f 6769 6e7a 022d 755a  cker..loginz.-uZ
+00000810: 1244 4f43 4b45 5248 5542 5f55 5345 524e  .DOCKERHUB_USERN
+00000820: 414d 457a 022d 705a 1244 4f43 4b45 5248  AMEz.-pZ.DOCKERH
+00000830: 5542 5f50 4153 5357 4f52 44fa 0964 6f63  UB_PASSWORD..doc
+00000840: 6b65 722e 696f 2903 7237 0000 005a 066c  ker.io).r7...Z.l
+00000850: 6f67 6f75 7472 3900 0000 7229 0000 0072  ogoutr9...r)...r
+00000860: 2a00 0000 290f 722d 0000 0072 1000 0000  *...).r-...r....
+00000870: 722e 0000 0072 0d00 0000 720f 0000 00da  r....r....r.....
+00000880: 0876 6572 7369 6f6e 7372 3600 0000 7231  .versionsr6...r1
+00000890: 0000 00da 1470 756c 6c5f 6966 5f6e 6f74  .....pull_if_not
+000008a0: 5f65 7869 7374 656e 7472 0400 0000 7203  _existentr....r.
+000008b0: 0000 0072 1b00 0000 721c 0000 0072 0500  ...r....r....r..
+000008c0: 0000 7216 0000 0029 0472 0700 0000 7222  ..r....).r....r"
+000008d0: 0000 0072 3500 0000 7234 0000 0072 1800  ...r5...r4...r..
+000008e0: 0000 7218 0000 0072 1900 0000 da0d 696d  ..r....r......im
+000008f0: 675f 646f 636b 6572 6875 623f 0000 0073  g_dockerhub?...s
+00000900: 2e00 0000 0c05 0201 1401 04ff 0403 0c01  ................
+00000910: 06ff 0e03 0a01 0201 0202 0201 0201 0801  ................
+00000920: 0201 0801 0201 02f9 04ff 0a0b 0c01 0a01  ................
+00000930: 0e01 723c 0000 0029 1272 1b00 0000 7212  ..r<...).r....r.
+00000940: 0000 00da 0674 7970 696e 67da 0274 705a  .....typing..tpZ
+00000950: 265f 636f 6d70 6f6e 656e 7473 2e5f 7061  &_components._pa
+00000960: 796c 6f61 642e 5f64 6f63 6b65 725f 6578  yload._docker_ex
+00000970: 6563 7574 6f72 7372 0300 0000 7204 0000  ecutorsr....r...
+00000980: 0072 0500 0000 da10 5f70 726f 746f 5f6e  .r......_proto_n
+00000990: 616d 6573 7061 6365 7206 0000 0072 1a00  amespacer....r..
+000009a0: 0000 7221 0000 00da 0341 6e79 da05 556e  ..r!.....Any..Un
+000009b0: 696f 6e72 2c00 0000 da08 5365 7175 656e  ionr,.....Sequen
+000009c0: 6365 7233 0000 0072 3c00 0000 7218 0000  cer3...r<...r...
+000009d0: 0072 1800 0000 7218 0000 0072 1900 0000  .r....r....r....
+000009e0: da08 3c6d 6f64 756c 653e 0100 0000 7336  ..<module>....s6
+000009f0: 0000 0008 0108 0108 010c 020c 010c 010c  ................
+00000a00: 0112 0312 1302 0a02 0102 ff04 0202 fe12  ................
+00000a10: 0302 fd02 040a fc02 1602 0102 ff04 0202  ................
+00000a20: fe02 0302 fd02 040e fc                   .........
```

### Comparing `adaux-2.1.1/source/adaux/src/payload/python/functions.py` & `adaux-2.2.0/source/adaux/src/payload/python/functions.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,24 +37,31 @@
     payload = aux.payload.lookup["gitlab-release-run"]
     payload.run()
 
 
 def tag(
     aux: _ProtoNamespace,  # pylint: disable=unused-argument
     deps: tp.Any,
-    tag: str,  # pylint: disable=redefined-outer-name
+    tags: tp.Union[str, tp.Sequence[str]],  # pylint: disable=redefined-outer-name
 ) -> None:
+    if isinstance(tags, str):
+        tags = [tags]
+
     if len(deps) != 1:
         raise RuntimeError(
-            f"tag job for {tag} should have exactly 1 dependency, not {len(deps)}!"
+            f"tag job for {tags} should have exactly 1 dependency, not {len(deps)}!"
         )
-    tag = tag.format(version=aux.project.version)
-    local_tag, release_tag = deps[0].executor.tag_and_upload(tag)
-    print("uploaded", local_tag)
-    print("   -> to", release_tag)
+    last_local_tag = ""
+    for tag in tags:  # pylint: disable=redefined-outer-name
+        tag = tag.format(version=aux.project.version, branch=aux.gitlab.current_branch)
+        local_tag, release_tag = deps[0].executor.tag_and_upload(tag)
+        if last_local_tag != local_tag:
+            last_local_tag = local_tag
+            print("uploaded", local_tag)
+        print("   -> to", release_tag)
 
 
 def img_dockerhub(
     aux: _ProtoNamespace,
     deps: tp.Any,
     release_tag: str,
 ) -> None:
```

### Comparing `adaux-2.1.1/source/adaux/src/pre-commit/add_copy_right.py.jinja2` & `adaux-2.2.0/source/adaux/src/pre-commit/add_copy_right.py.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.1.1/source/adaux/src/pre-commit/config.yaml.jinja2` & `adaux-2.2.0/source/adaux/src/pre-commit/config.yaml.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.1.1/source/adaux.egg-info/SOURCES.txt` & `adaux-2.2.0/source/adaux.egg-info/SOURCES.txt`

 * *Files identical despite different names*

