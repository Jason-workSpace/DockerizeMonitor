# Run arb-monitor docker

build docker:
```
docker build -t faucet .
```
we should modify env_docker.smaple and copy to env_docker
```
cp env_docker.smaple env_docker
```
then start:
```
docker run --name={nitro_faucet} --env-file=./env_docker -d faucet start
```

