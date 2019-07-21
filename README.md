# Cart gRPC service
This source file is used to generate Cart Server interface and Cart client.
Generated code is imported by other services, please keep it backwards compatible.

## Tools
[Install proto compiler and Go related tools](https://github.com/golang/protobuf#installation) first.

## Generate Go code
Assuming that projects directories are located next to each other.

```
{projects}/github.com/cooldryplace
	/cart
	/certs
	/proto
	/proto-sources
```

Please use this command to compile proto files.
`protoc -I ./ cart_service.proto --go_out=plugins=grpc:./../../..`
