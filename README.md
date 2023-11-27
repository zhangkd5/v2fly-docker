# Docker Fly

Fork of the original v2fly/docker repo to build docker images in personal DockerHub. 

## Usage

```bash
docker run --rm v2fly/v2fly-core help

docker run --name v2ray v2fly/v2fly-core $v2ray_args (help, run etc...)

docker run -d --name v2ray -v /path/to/config.json:/etc/v2ray/config.json -p 10086:10086 v2fly/v2fly-core run -c /etc/v2ray/config.json 

# If you want to use v5 format config
docker run -d --name v2ray -v /path/to/config.json:/etc/v2ray/config.json -p 10086:10086 v2fly/v2fly-core run -c /etc/v2ray/config.json -format jsonv5
```
