# grpc-chat-server
A simple gRPC streaming chat server using Go

## Echo Proto
- To compile run the following
```sh
cd echo
protoc -I chat chat/chat.proto --go_out=plugins=grpc:chat
```
## Echo Server
- To run the server
```sh
cd server
go run main.go
```

## Echo Client
- To run the server
```sh
cd client
go run main.go
```