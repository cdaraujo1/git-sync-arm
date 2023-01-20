# git-sync ARM.

Git-sync image for ARM processors.

> Based on [openweb](https://github.com/openweb-nl/git-sync) project. These are the same code but built for ARM.

Steps to build:
1 - Clone the repository in the desired branch tag.

`git clone --branch master https://github.com/openweb-nl/git-sync.git`

2 - Build the image.

>  Recommended to build directly from an ARM instance (you can try Oracle Cloud Ampere instances)

```sh
Building from ARM.

$ docker build -t <repo>/git-sync:0.0.1-arm .
```

Or building using _buildx_

```shell
Building from x84.

$ docker buildx build --platform linux/arm64 -t <repo>/git-sync:0.0.1-arm .
```

----

## See on [Dockerhub](https://hub.docker.com/r/cdaraujo/git-sync)
