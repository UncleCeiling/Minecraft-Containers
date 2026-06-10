# Minecraft Containers

> This repo is intended to allow me to easily track my `compose.yaml` files for hosting Minecraft servers.

## General Steps

1. Install Docker and Docker Compose.

2. Create a folder for the server.

3. Create `compose.yaml` using generator.

4. Add `compose.yaml` to folder.

- Create `data` folder in server folder.
- Add world-folder to data folder.

5. Return to the folder with the `compose.yaml` and run the following command:

```sh
docker compose up
```

## Using a `compose.yaml` in this repo

1. Clone this repo to the computer you are hosting on.
2. `cd` to the folder of the server you want to run.
3. **[optional]** `mkdir data` and copy any world files you want to carry over. You may need to edit the `level` parameter of the corresponding `compose.yaml`.
4. Run `docker compose up`.
5. If you get an `API` error; create a `.env` file and add the appropriate key, making sure the environment variable is correct (correctly escaped/labelled) and try again.
6. In the case of API rate limits, disable the restart policy until rate limits lift.

## Docker Cheat Sheet

|                             Command | Usage                                                                |
| ----------------------------------: | :------------------------------------------------------------------- |
|         `docker compose up --build` | Build and run the `compose.yaml` file (use inside folder with file). |
|                         `docker ps` | List currently running containers.                                   |
| `docker exec -it <CONTAINER ID> sh` | Start an interactive shell with a given container.                   |
|        `docker stop <CONTAINER ID>` | Stop the shell.                                                      |

## Resources

[itzg minecraft docker image](https://docker-minecraft-server.readthedocs.io/)

[compose.yaml generator](https://setupmc.com/java-server/)

## Modpacks

[Homestead](https://www.curseforge.com/minecraft/modpacks/homestead-cozy)

[StoneBlock4](https://www.curseforge.com/minecraft/modpacks/ftb-stoneblock-4)
