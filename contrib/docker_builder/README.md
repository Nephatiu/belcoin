# Dockerfile for building belcoin binaries.

Now, you can build your own belcoin files on all systems with docker and do it easy without installing depends on your system.

## How:

### Build docker image

```
sudo docker build .
```

### Run docker container

Builder will return HASH of image
Example:
Successfully built 9bbff825d50f

```
sudo docker run -it -v ~/path/to/belcoin/folder:/belcoin 9bbff825d50f
```

If your system uses SELINUX you may use --privileged=true key

```
sudo docker run --privileged=true -it -v ~/development/belcoin:/belcoin 9bbff825d50f
```

See belcoin-qt file in used belcoin folder and belcoind file in src subfolder.