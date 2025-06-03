# Dockerfile

For building klipper mcu and btt eddy firmware.

## Publishing docker file

```
docker build . -t pellcorp/klipper-fw-build
docker login
docker push pellcorp/klipper-fw-build
```
