# grafana-volkovlabs-app

# 🚀 Volkov Labs Application for @grafana 🚀


https://github.com/coding-to-music/grafana-volkovlabs-app

From / By https://github.com/volkovlabs/volkovlabs-app


## Environment variables:

```java
```

## user interfaces:

- Grafana http://localhost:3000

## GitHub

```java
git init
git add .
git remote remove origin
git commit -m "first commit"
git branch -M main
git remote add origin git@github.com:coding-to-music/grafana-volkovlabs-app.git
git push -u origin main
```

## Running 

```
yarn install
yarn build
yarn start
```

See what is running

```
docker ps
```

Output

```
CONTAINER ID   IMAGE                           COMMAND                  CREATED         STATUS                          PORTS                    NAMES
4d745d18dfa3   grafana-volkovlabs-app_nginx    "/docker-entrypoint.…"   5 minutes ago   Restarting (1) 30 seconds ago                            nginx
56cc6c12076d   ghcr.io/volkovlabs/app:latest   "/run.sh"                5 minutes ago   Up 5 minutes                    0.0.0.0:3000->3000/tcp   grafana
```

View the docker run logs

```
nginx exited with code 1
nginx      | 10-listen-on-ipv6-by-default.sh: info: /etc/nginx/conf.d/default.conf differs from the packaged version
nginx      | /docker-entrypoint.sh: Launching /docker-entrypoint.d/20-envsubst-on-templates.sh
nginx      | 20-envsubst-on-templates.sh: Running envsubst on /etc/nginx/templates/default.conf.template to /etc/nginx/conf.d/default.conf
nginx      | /docker-entrypoint.sh: Launching /docker-entrypoint.d/30-tune-worker-processes.sh
nginx      | /docker-entrypoint.sh: Configuration complete; ready for start up
nginx      | 2023/04/18 22:44:33 [emerg] 1#1: host not found in upstream "host.docker.internal" in /etc/nginx/conf.d/default.conf:7
nginx      | nginx: [emerg] host not found in upstream "host.docker.internal" in /etc/nginx/conf.d/default.conf:7
nginx exited with code 1
```

# Volkov Labs Application for Grafana

![Application](https://raw.githubusercontent.com/volkovlabs/volkovlabs-app/main/img/app.png)

![Grafana 9](https://img.shields.io/badge/Grafana-9.4.7-orange)
[![YouTube](https://img.shields.io/badge/YouTube-Channel-red)](https://youtube.com/@volkovlabs)
![CI](https://github.com/volkovlabs/volkovlabs-app/workflows/CI/badge.svg)
[![codecov](https://codecov.io/gh/VolkovLabs/volkovlabs-app/branch/main/graph/badge.svg)](https://codecov.io/gh/VolkovLabs/volkovlabs-app)
[![CodeQL](https://github.com/VolkovLabs/volkovlabs-app/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/VolkovLabs/volkovlabs-app/actions/workflows/codeql-analysis.yml)

## Introduction

The Volkov Labs Application includes a Docker image and Application plugin with information about Volkov Labs maintained Grafana plugins.

## Requirements

- Grafana 9.0+ is required.

## Docker image

We use custom build Docker image for all our projects and keep it up-to-date with the latest version of Grafana.

```sh
docker pull ghcr.io/volkovlabs/app:latest
```

## Bundle

Application plugin includes.

- [RSS/Atom data source](https://volkovlabs.io/plugins/volkovlabs-rss-datasource)
- [Dynamic text panel](https://volkovlabs.io/plugins/volkovlabs-dynamictext-panel)

## Feedback

We love to hear from you. There are various ways to get in touch with us:

- Ask a question, request a new feature, and file a bug with [GitHub issues](https://github.com/volkovlabs/volkovlabs-app/issues/new/choose).
- Sponsor our open-source plugins for Grafana with [GitHub Sponsor](https://github.com/sponsors/VolkovLabs).
- Star the repository to show your support.

## License

Apache License Version 2.0, see [LICENSE](https://github.com/volkovlabs/volkovlabs-app/blob/main/LICENSE).
