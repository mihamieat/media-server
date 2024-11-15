# my media server

## overview 👀

this is my media server app that runs with docker.

the app contains services such as jellyfin, deluge and jackett.

## install ⚙

make sure to have docker engine installed as well as docker command lines.

### set environment variables

the application needs to have a `.env` file. create it and set the following mendatory environment variables:

| Key                         | value                                             |
| --------------------------- | ------------------------------------------------- |
| JELLYFIN_PublishedServerUrl | your server url (typically http://127.0.0.1:8096) |
| PUID                        | the process user id (1000)                        |
| PUID                        | the process group id (1000)                       |
| TZ                          | time zone (Eruope/Paris)                          |

### docker compose 🐳

```sh
./run.sh
```

## run 🚀

### jellyfin

access to jellyfin interface to your server url and port `8096`

### deluge

access to deluge interface to your server url and port `8112`

default deluge password is `deluge`. it is advised to change it.

### jackett

access to jacket interface to your server url and port `9117`

## stop the services

```sh
./stop.sh
```