# sentry config
sentry deploy

# setps
```
mkdir -p /opt/services/sentry-config
mkdir -p /mnt/services/sentry/logs
git clone https://github.com/huhulab/sentry-config /opt/services/sentry-config
pip install -r deps.txt
cd /opt/services/sentry-config/deploy
cp config.toml.sample config.toml
vim config.toml
...
python manager.py config
python manager.py supervisor
```
