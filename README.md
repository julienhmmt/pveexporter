# pveexporter

a simple ansible role to install prometheus-pve-exporter into a python virtualenv.

requirements :

- python3-pip
- python3-virtualenv

some vars are needed :

- `pve_exporter_conf_path`: = path where files and virtualenv will be created
- `pve_exporter_group`: = user for pve_exporter process
- `pve_exporter_user`: = group for pve_exporter process
- `pve_exporter_proxmox_user`: = user created in your pve cluster
- `pve_exporter_token_name`: = create a token for your user, in "Permissions/API Token"
- `pve_exporter_token_value`: = value of the token

to test, simply type this : `curl http://localhost:9221/pve?target=cluster.domain.local:8006?cluster=1&node=0

