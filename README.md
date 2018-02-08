# Workspace CPU Bench


OS: `lsb_release -a`

sudo apt update
sudo apt install sysbench

sysbench --test=cpu --cpu-max-prime=20000 --num-threads=2 run

| Workspace | RAM | OS | CPU | Performance | Notes |    
| ----- | ----- | ----- | ----- | ----- | ----- |
| cs50.io  | 512MB | 14.04.5 | 1m20s | |