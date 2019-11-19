# ai-arena-client-gui

1: Download the Docker image
```docker pull m1ndgames/ai-arena-client-gui```

2: Run the Docker Container
```docker run -p 127.0.0.1:8080:8080 m1ndgames/ai-arena-client-gui```

3: Open a Browser on the Host and go to http://127.0.0.1:8080

## Notes
### Mounting Bot directories
If you want to mount directories from the host system you can add the parameter
```-v <host_dir>:<container_dir>```
Example:
```docker run -v C:\Bots:/home/aiarena/StarCraftII/Bots -p 127.0.0.1:8080:8080 m1ndgames/ai-arena-client-gui```
