# Dev Container Workflow for csharp

## References

- https://github.com/marcel-dempers/docker-development-youtube-series/
- https://www.youtube.com/watch?v=EdmKENqnQUw

## Code v1

```bash
docker-compose up

# Attach to running container using VS Code or
docker compose exec csharp bash

# or this command 
docker exec -it csharp bash
```

## Code v2

```bash

   15  mkdir src
   16  cd src/
   17  dotnet new webapp

# Add the following line to program.cs
...
WebHost.CreateDefaultBuilder(args)
                .UseUrls("http://*:5000")
...

   18  dotnet build
   dotnet run

# navigate to http://localhost:5000
```