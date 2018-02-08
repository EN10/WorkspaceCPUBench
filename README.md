# Workspace CPU Bench

Benchmarking free online workspaces

### Info

OS: `lsb_release -a`    
CPU `less /proc/cpuinfo`

### Install

    sudo apt update
    sudo apt install sysbench
    sysbench --version

### Run

    sysbench --test=cpu --cpu-max-prime=20000 --num-threads=2 run

### Benchmarks

| Workspace | CPU | RAM | OS | sysbench | Threads | Total Time |   
| -------- | ----- | ---- | ------- | ------- | ------ | ----- |
| cs50.io  | 2.50GHz | 512MB | 14.04.5 | 0.4.12 | 1 | 28.8560s |
| cs50.io  | 2.50GHz | 512MB | 14.04.5 | 0.4.12 | 2 | 20.9147s |
| cs50.io  | 2.50GHz | 512MB | 14.04.5 | 0.4.12 | 4 | 21.8916s |