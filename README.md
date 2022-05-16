# Dotnet templates for grpc-csharp-course

This repository contains two templates for creating gRPC project faster during my Udemy course (repo: [grpc-csharp-course](https://github.com/Clement-Jean/grpc-csharp-course))

You should clone this repository in a folder called `working` and to install the templates run:

```
dotnet new --install working/templates/grpcserver
dotnet new --install working/templates/grpcclient
```

and to uninstall:

```
dotnet new --uninstall working/templates/grpcserver
dotnet new --uninstall working/templates/grpcclient
```

After having installed the templates, you will be able to run the following commands:

```
dotnet new grpcserver
dotnet new grpcclient
```

## Why ?

The original `grpc` template provided with the dotnet CLI comes with a lot of boilerplate and this is quite annoying, especially when recording a online course. Furthermore, the dotnet CLI does not provide a way to create a client easily. Even though my client template is a basic console app, this could be replicated easily to other more complex setups.

## grpcserver

This template is a bare bone grpc server without any proto file and any service. It contains a dependency to `Grpc.AspNetCore`.

## grpcclient

This template is a console project having dependency to `Google.Protobuf`, `Grpc.Net.Client` and `Grpc.Tools`.