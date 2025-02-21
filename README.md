```bash
# put wireguard config to wg.conf
cp env_template env
vim env
(set -a; source ./env; envsubst < shadowsocks.json.template > shadowsocks.json; envsubst < config.alloy.template > config.alloy)
docker compose up -d
```
