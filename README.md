# ai-arena-client-gui
This Container provides a full working StarCraft II linux setup including Java 11, Wine, DotNetCore and Python 3.7 including modules necessary to run the most Bots.

You will be able to test your Bot locally using a Browser based GUI, either against other Bots on your System or Publicly downloadable Bots from the ai-arena SC2 ladder. (https://ai-arena.net)

## Guide
1: Download the Docker image
```docker pull m1ndgames/ai-arena-client-gui```

2: Run the Docker Container
```docker run -p 127.0.0.1:8080:8080 m1ndgames/ai-arena-client-gui```

3: Open a Browser on the Host and go to http://127.0.0.1:8080

## Notes
### Mounting Bot directories
If you want to mount directories from the host system you can add the parameter ```-v <host_dir>:<container_dir>```

Example:

```docker run -v C:\Bots:/home/aiarena/StarCraftII/Bots -p 127.0.0.1:8080:8080 m1ndgames/ai-arena-client-gui```
