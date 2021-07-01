# Minecraft server in Docker Compose

## Quickstart

```bash
# Start a minecraft server
make run
# Start a minecraft server with a specific compose project and randomly assigned port
make run project=minecraft1 port=
# Start a minecraft server with a specific compose project on port 5000
make run port=5000
# Stop minecraft and delete the world volume
make clean volumes=true
# Just build the image
make build
```
