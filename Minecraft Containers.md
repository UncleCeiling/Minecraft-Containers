# Minecraft Containers

## Resources

[itzg minecraft docker image](https://docker-minecraft-server.readthedocs.io/)
[compose.yaml generator](https://setupmc.com/java-server/)

## Steps

1. Install Docker and Docker Compose.

2. Create a folder for the server.

3. Create `compose.yaml` using generator.

4. Add `compose.yaml` to folder.

- Create `data` folder in server folder.
- Add world-folder to data folder.

5. Return to the folder with the `compose.yaml` and run the following command:

```sh
docker compose
```

## Docker Cheat Sheet

|                             Command | Usage                                                                |
| ----------------------------------: | :------------------------------------------------------------------- |
|         `docker compose up --build` | Build and run the `compose.yaml` file (use inside folder with file). |
|                         `docker ps` | List currently running containers.                                   |
| `docker exec -it <CONTAINER ID> sh` | Start an interactive shell with a given container.                   |
|        `docker stop <CONTAINER ID>` | Stop the shell.                                                      |

## Modpacks

[Homestead](https://www.curseforge.com/minecraft/modpacks/homestead-cozy)

[StoneBlock4](https://www.curseforge.com/minecraft/modpacks/ftb-stoneblock-4)
