## Build an Image ##

```docker build --tag nci02 .```


## Run an image ##

```docker run --name ncilab02 -p 8090:8080 nci02```

## Run the curl command ##

This transfers ETH:

```curl --header "Content-Type: application/json" --request POST --data '{"address":"0x9b9a8Ff1e5A8945043d31470BDb843FD0A91eA33", "amount":"0.05"}' http://localhost:8090/eth```

This transfers token:

```curl --header "Content-Type: application/json" --request POST --data '{"address":"0x9b9a8Ff1e5A8945043d31470BDb843FD0A91eA33"}' http://localhost:8090/token```

