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
- Run multiple clients on different terminal and start chat
```sh
cd client
go run main.go 127.0.0.1:8080 john 
```

```sh
cd client
go run main.go 127.0.0.1:8080 peter 
```

```sh
cd client
go run main.go 127.0.0.1:8080 abdul 
```