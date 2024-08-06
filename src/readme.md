# WeatherForecastApi

[![.NET](https://github.com/mib96/devops-project-cicd-app/actions/workflows/dotnet.yml/badge.svg)](https://github.com/mib96/devops-project-cicd-app/actions/workflows/dotnet.yml)

## Prerequisites

* .NET 8 SDK

## Commands

The below commands are assumed to be executed in the context of `src` directory (unless stated otherwise).

### Running app

`dotnet run`

### Building

`dotnet build`

### Running tests

Go to test project directory and run:

`dotnet test`

### Producing publishable artifacts

`dotnet publish WeatherForecastApi.Web -c Release --output ./build_output`

The output will be located in `src/build_output` directory.
