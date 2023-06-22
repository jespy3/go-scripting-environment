# go-scripting-environment

Copy this repo to have a good foundational docker-based go scripting environment using a command like:
```
git clone git@github.com:jespy3/go-scripting-environment.git
cp -r ./go-scripting-environment ./new-repo-name
cd new-repo-name
rm -rf .git      # to disassociate the 'go-scripting-environment' git files
```

## Setup

Ensure `docker compose` is available on current version of docker.

Run
```
docker compose up -d
```

Then
```
docker compose exec box bash
```

## Running the script

In the container, run:
```
go run hello-world.go

# OR, as a executable
go build hello-world.go
./hello-world
```
