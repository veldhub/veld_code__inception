# ![veld code](https://raw.githubusercontent.com/veldhub/.github/refs/heads/main/images/symbol_V_letter.png) veld_code__inception

This repo contains [code velds](https://zenodo.org/records/13322913) encapsulating an 
[INCEpTION](https://github.com/inception-project/inception) instance with an accompanying mariadb 
service for persistence.

## requirements

- git
- docker compose (note: older docker compose versions require running `docker-compose` instead of 
  `docker compose`)

## how to use

This code veld may be integrated into a chain veld, or used directly by adapting the configuration 
within its yaml file and using the template folders provided in this repo. Open the veld yaml file 
for more information.

**[./veld.yaml](./veld.yaml)** 

Launches an inception instance. Inception metadata is stored under
[./data/inception_app/](./data/inception_app/) and the mariadb content under 
[./data/inception_db/](./data/inception_db/) .

```
docker compose -f veld.yaml up
```

