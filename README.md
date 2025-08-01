# Netdata Monitoring with Docker

## Description
This project demonstrates how to monitor system resources using Netdata running in a Docker container.

## Steps
1. Install Docker from: https://www.docker.com/products/docker-desktop/
2. Run Netdata container:
```bash
docker run -d --name=netdata -p 19999:19999 --cap-add SYS_PTRACE --security-opt apparmor=unconfined netdata/netdata
```
3. Open your browser and visit: http://localhost:19999
4. Take a screenshot of the dashboard and save it in the `screenshot/` folder.

## Optional
Use `docker_run_netdata.sh` script to launch Netdata quickly.

## Screenshot
See `screenshot/netdata_dashboard.png`
