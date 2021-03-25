# .NET Core Sample application

This is .NET core sample based on [this tutorial](https://dotnet.microsoft.com/learn/aspnet/hello-world-tutorial/intro).

## .NET Core installation

Installed from .Net Core [download site](https://dotnet.microsoft.com/download/dotnet-core/5.0)

## Build and Run locally

```bash
dotnet run
```

## Deploy

### Create app using dotnet platform
```bash
shipa app create dotnet-sample dotnet -t admin
```

It creates an app with name `dotnet-sample` using `dotnet` platform. 

### Deploy

```bash
shipa app deploy -a dotnet-sample -f .
```
Option `-f .` tells shipa to deploy all files from the current folder

After deployment run `shipa app list`

```text
+---------------+-----------+-----------------------------------------------+
| Application   | Units     | Address                                       |
+---------------+-----------+-----------------------------------------------+
| dashboard     | 1 started | http://dashboard.10.100.10.20.shipa.cloud     |
+---------------+-----------+-----------------------------------------------+
| dotnet-sample | 1 started | http://dotnet-sample.10.100.10.20.shipa.cloud |
+---------------+-----------+-----------------------------------------------+
```
Access your app at `http://dotnet-sample.10.100.10.20.shipa.cloud`

