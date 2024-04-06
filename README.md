# Docker-practice-demo-02
Create a docker compose with mongo-db and mongo-express containers

```cmd
docker-compose -f docker-compose.yaml up
```
-f stands for file and docker-compose.yaml is the file name and up stand for create and start containers.

-------------------------------
## Volumes

Randomly it might generate a new volume for the container and there is no data persistence of the data. When we are creating data volumes there is data persistence for the data. Even if we stop the container the data will be always going to be there.

Mount container data into a permanent path instead of mounting them as a bind mount. If we run docker-compose without volumes, data will mout as bind mount, and data changes we are doing will not be saved once we down the compose and up again. It will mount to another volume. But when we specify a volume data will be mounted permanently to that volume and data will not be lost.

Here/data/db is the default volume mount path of Mongo-db. If we are using another container it will change according to the container or image.
