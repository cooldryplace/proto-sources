# Cart gRPC service
This source file is used to generate Cart Server interface and Cart client.
Generated code is imported by other services, please keep it backwards compatible.

## Generate Go code
`protoc -I ./ cart_service.proto --go_out=plugins=grpc:./..`
