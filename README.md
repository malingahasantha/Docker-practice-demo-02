# Docker-practice-demo-02
Create a docker compose with mongo-db and mongo-express containers

docker-compose -f docker-compose.yaml up

-f stands for file and docker-compose.yaml is the file name and up stand for create and start containers.

-------------------------------
Volumes

Mount container data into a permanent path instead of mounting them as a bind mount. If we run docker-compose without volumes data will mout as bind mount and data changes we are doing will not be saved once we down the compose and up again. It will mount to another volume. But when we specify a volume data will be mounted permanently to that volume and data will not be lost.
