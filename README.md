# MTA:SA Docker Image

This is a dockerfile config to set up a MTA:SA Server on docker.

## Links
- https://hub.docker.com/r/ciber96/mtasa-docker

## Installation for Use Out of the Box
``bash
docker pull ciber96/mtasa-docker
docker run \
-p 22003:22003 \
-p 22005:22005 \
-p 22126:22126 \
-d ciber96/mtasa-docker
```


## Installation(Dev)

```bash
git clone https://github.com/ciber96/mtasa-docker.git
cd mtasa-docker
docker build --tag 'mtaserver:latest' .
```

## Usage

```bash
docker run \
-p 22003:22003 \
-p 22005:22005 \
-p 22126:22126 \
-d mtaserver
```
## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## Known Issues
- Output of Server is not visible until we quit with CTRL+C
