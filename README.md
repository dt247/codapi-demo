# codapi demo

## install

download `codapi` from [here](https://github.com/nalgeon/codapi/releases/tag/0.6.0) and place the binary in this folder.

## build images

you can build the preferred sandbox environment

```bash
docker build --file images/alpine/Dockerfile --tag codapi/alpine:latest images/alpine
docker build --file images/python/Dockerfile --tag codapi/python:latest images/python
docker build --file images/cling/Dockerfile --tag codapi/cling:latest images/cling
docker build --file images/cpp/Dockerfile --tag codapi/cpp:latest images/cpp
docker build --file images/sqlite/Dockerfile --tag codapi/sqlite:latest images/sqlite
```

## configuration

- `configs/config.json` for common configuration.
- `configs/boxes.json` for image settings
- `configs/commands/<lang>.json` for command support for different images

## start service

```bash
./codapi
```

## reference

- https://github.com/nalgeon/codapi/tree/0.6.0/docs