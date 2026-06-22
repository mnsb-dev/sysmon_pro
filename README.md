# SysMon Pro

Real-time system monitoring dashboard for headless Linux servers.

## What it monitors
- CPU load, frequency, per-core breakdown, temperature sensors
- Memory — real usage, buffers, cache, swap
- Disk partitions with WARNING/CRITICAL threshold badges
- Disk I/O — live MB/s rates + cumulative totals
- Network interfaces and active connections
- Docker container stats (parallelized, non-blocking)
- API collector latency panel (self-monitoring)

## Alerting
Threshold-based Discord webhook alerts with cooldown logic and 
recovery notifications. Configure via CONFIG in sysmon_pro.py.

## Stack
Python · psutil · Docker SDK · threading · Discord API · vanilla JS/Canvas

## Requirements
- Linux (Ubuntu Server 22.04/24.04 tested)
- Python 3.10+
- pip install psutil docker

## Run
python3 sysmon_pro.py
## Dashboard: http://localhost:9400

## Documentation
See [SYSMON_PRO.pdf](SYSMON_PRO.pdf) for annotated screenshots of every dashboard section running on a real Ubuntu Server.
