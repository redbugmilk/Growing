# Get start for javascript environment

I will use [loopback 4](https://loopback.io/doc/en/lb4/Getting-started.html) to do the get-starting for a backend for the javascript stack.

## Install

Install the CLI globally:
```
npm i -g @loopback/cli
```

## Getting start
Run to create a project:
```
lb4 app
```

Added the follow configuration:

```
? Project name: getting-started
? Project description: Getting started tutorial
? Project root directory: (getting-started)
? Application class name: StarterApplication
? Select features to enable in the project:
❯◉ Enable eslint: add a linter with pre-configured lint rules
 ◉ Enable prettier: install prettier to format code conforming to rules
 ◉ Enable mocha: install mocha to run tests
 ◉ Enable loopbackBuild: use @loopback/build helpers (e.g. lb-eslint)
 ◉ Enable vscode: add VSCode config files
 ◉ Enable docker: include Dockerfile and .dockerignore
 ◉ Enable repositories: include repository imports and RepositoryMixin
 ◉ Enable services: include service-proxy imports and ServiceMixin
```

Run the server:
```sh
cd getting-start && npm start
```

Server is running at:
```
 http://[::1]:3000
```

Call the ping:
```
http://[::1]:3000/ping
```

Got the answer:
```json
{
    "greeting": "Hello from LoopBack",
    "date": "2019-11-10T21:18:09.026Z",
    "url": "/ping",
    "headers": {
        "user-agent": "PostmanRuntime/7.19.0",
        "accept": "*/*",
        "cache-control": "no-cache",
        "postman-token": "64906c2e-7fa6-47be-8048-b4c3de6fa6d0",
        "host": "[::1]:3000",
        "accept-encoding": "gzip, deflate",
        "connection": "keep-alive"
    }
}
```