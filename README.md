# Workspace CPU Bench

Benchmarking free online workspaces
Based on [TensorFlowForPoets](https://github.com/EN10/TensorFlowForPoets#benchmarks)

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
| -------- | ------- | ---- | ------- | ------- | ------ | ----- |
| cs50.io | 2.50GHz | 512MB | 14.04.5 | 0.4.12 | 1 | 28.8560s |
| cs50.io | 2.50GHz | 512MB | 14.04.5 | 0.4.12 | 2 | 20.9147s |
| cs50.io | 2.50GHz | 512MB | 14.04.5 | 0.4.12 | 4 | 21.8916s |
| codenvy.io | E5-2686 v4 @ 2.30GHz | 3072MB | 16.04.3 | 0.4.12 | 1 | 28.0834s |
| codenvy.io | E5-2686 v4 @ 2.30GHz | 3072MB | 16.04.3 | 0.4.12 | 2 | 14.2357s |
| codenvy.io | E5-2686 v4 @ 2.30GHz | 3072MB | 16.04.3 | 0.4.12 | 4 | 8.5462s |
| codenvy.io | E5-2686 v4 @ 2.30GHz | 3072MB | 16.04.3 | 0.4.12 | 8 | 8.5361s |