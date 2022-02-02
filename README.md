# Aim of repo

- To create easily reusable web app project templates consisting of
  - api
  - frontend
  - proxy
  - database
- To store production ready docker-compose and Dockerfile configurations that can be used for development

# Supported combinations

- api
  - nestjs
  - go (WIP)
- frontend
  - sveltekit
  - nextjs (WIP)
- database
  - postgreSQL
- proxy
  - Caddy

# Instructions

Currently only nestjs and sveltekit combination is supported.
To start, run

```bash
cd apis/nestjs
# install api dependencies
yarn

cd ../../frontends/sveltekit
# install frontend dependencies
yarn

cd ../../
# start docker-compose
docker-compose up -d
```
