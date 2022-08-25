# Run arb-monitor docker
Since arb-monitor repository is private, so it should download it to local first:
```
git clone https://github.com/OffchainLabs/arb-monitoring.git
```
then build docker:
```
docker build -t arb-monitor .
```
and when start a containner, we should clarify the chain id in .env
then start like (start protocol_events as example):
```
docker run --name=protocol_events-421611 --env-file=./env_docker -d arb-monitor protocol_events
```
we can also change the protocol_envents to: `bridge`, `retryables`, `ts-node ./lib/arbiscan_blocks.ts`, `ts-node ./lib/arbiscan_batches.ts`

