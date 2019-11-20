# Get start for .Net environment

## Links to follow
- https://dotnet.microsoft.com/learn/aspnet/microservice-tutorial/intro
- https://www.youtube.com/watch?v=04IP3Yl8-64&list=PLdo4fOcmZ0oW8nviYduHq7bmKode-p8Wy
- https://docs.microsoft.com/pt-br/aspnet/core/tutorials/first-web-api?view=aspnetcore-3.0&tabs=visual-studio

## Experience 
It was really fast to do the get start, with some useful information. However, I miss some information about the detail:

File Structure:
```
  | Dependecies
  | Controllers
    | WeatherForecastController.cs
  | Properties
    | launchsettings.json
  | .dockerignore
  | appsettings.json
  | Dockerfile
  | Program.cs
  | Startup.cs
  | WeatherForecast.cs
```

File\Directories description:
- **Dependecies**: internal projects, or nugets libraries, or external libraries(native or not). (javascript: /nodes_modules);
- **Controllers**: directory where all controllers are kept. Controllers are the classes where the endpoints of the API are implemented;
- **Properties**: directory where project properties are kept. Examples, environment settings and launch settings;
- appsettings.json: app configurations according to environment;
- Program.cs: main of the project;
- Startup.cs: class where there application is configured, here you can add configuration for authentication, routing, authorization, dependency injection;
- WeatherForecast.cs: class with the model of the entity;
