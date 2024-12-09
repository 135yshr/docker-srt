# SRT Docker Image (Fork by 135yshr)

[![docker status](https://dockeri.co/image/135yshr/srt)](https://hub.docker.com/r/135yshr/srt)

This is a fork of the [SRT Docker Image](https://github.com/miyukki/srt-docker) created by [miyukki](https://github.com/miyukki).  
The project provides a lightweight [Haivision/srt](https://github.com/Haivision/srt) docker image based on Ubuntu.

Inside this container, you can execute the following binaries provided by Haivision/srt:
`srt-live-transmit`, `srt-file-transmit`, `srt-tunnel`, etc.

---

## Changes Made in This Fork
The following changes have been made from the original repository:
- Updated dependencies to support the latest version of Haivision SRT.
- Added new build options for customization.
- Improved documentation for building and running the Docker image.

---

## How to use

Run the Docker container using the prebuilt image `135yshr/srt`.

```sh
docker run -it --rm 135yshr/srt:latest srt-live-transmit udp://127.0.0.1:5000 srt://:60000
```

## How to build

Run make command with args.

```sh
DOCKER_TAG=v1.4.1 SRT_BRANCH=v1.4.1 make build
```

## Licence

[MIT](https://github.com/tcnksm/tool/blob/master/LICENCE)
This project is licensed under the [MIT License](https://github.com/135yshr/srt-docker/blob/main/LICENSE).
It retains the original license and copyright from the [miyukki](https://github.com/miyukki) repository.

## Credits

Original project by [miyukki](https://github.com/miyukki).
Forked and maintained by [135yshr](https://github.com/135yshr).
