Example of building Images

Building PHP Development Image:
```
docker run --rm -v ${PWD}:/work -w /work cgr.dev/chainguard/apko build apko.dev.yaml ghcr.io/realsamanrad/php:8.4-dev image-dev.tar
docker load < image-dev.tar
```

Building PHP Production Image:
```
docker run --rm -v ${PWD}:/work -w /work cgr.dev/chainguard/apko build apko.yaml ghcr.io/realsamanrad/php:8.4 image.tar
docker load < image.tar
```
