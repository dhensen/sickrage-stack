# Sickrage Stack

## Prerequisites
- docker
- docker-compose

## Usage
```
git clone git@github.com:dhensen/sickrage-stack.git
cd sickrage-stack
git submodule init
git submodule update
mkdir -p data/{complete,incomplete,series,watch}
docker-compose up -d
```

## Notes
If you want your data folder to reside elsewhere you can create specific symlinks or adjust the docker-compose.yml.
(Just keep in mind that the processes inside containers are running with UID=1000, see Todo)

### Todo
- make UID in sickrage and transmission dockerfiles variable
