```bash
cp env_template env
nano env
(set -a; source ./env; envsubst < xray.json.template > xray.json; envsubst < config.alloy.template > config.alloy)
docker compose up
```
