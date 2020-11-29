# Multi Docker

Multi docker is script to clone or pull git repository and up or down docker-compose from a config file

## Installation

The script dependencie is [GitPython](https://gitpython.readthedocs.io/en/stable/) to clone or pull automatic git repository.

**Install Git Python**
```bash
sudo apt-get install python3-pip
pip3 install gitpython
chmod +x multidocker
```

**copy config**
```
cp  docker-repositories.dist.json  docker-repositories.json
```

## Command

**Clone or pull git repository**
```bash
./multidocker --pull
```

**Docker Compose Up**
```bash
./multidocker --up
```

**Docker Compose Down**
```bash
./multidocker --down
```

**Select other config file**
```bash
./multidocker --config-file=path/to/your/file.json
```

**Helper**
```bash
./multidocker -h
 -h,  --help                 view this helper
 -d,  --debug                Debug script
      --config-file=         Path to config file, default=docker-config.yml
      --pull                 Clone or pull repositories in the config file
      --up                   Up docker compose repositories in the config file
      --down                 Down docker compose repositories in the config file
```





## Credits

Created by [Matthieu Beurel](https://www.mbeurel.com). Sponsored by [Nexboard](https://www.nexboard.fr).