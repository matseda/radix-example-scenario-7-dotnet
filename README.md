# Radix - dotnet - scenario 1

App with one container. No external back end dependencies. No storage. No secrets.

## Getting Started

This app was created with the command: `dotnet new webapp -o radix-example-scenario-1-dotnet`.


### Installing
To run the app you only need to have the Docker Engine.
```
git clone https://github.com/Statoil/radix-example-scenario-1-dotnet.git
cd radix-example-scenario-1-dotnet
docker build -t radix-example-scenario-1-dotnet .
docker run -d -p 5000:5000 --name radix-example-scenario-1-dotnet radix-example-scenario-1-dotnet
```
The app should then be available on [port 5000](http://localhost:5000/).

*If* you have **Docker Compose** installed you can use:
```
docker-compose up
```
to build and run the app.


## Deployment

For deployment please follow the getting started on the [Omnia radix wiki](https://radix-wiki.azurewebsites.net/doku.php/appdeveloper/gettingstarted).

**Note**: The radix platform uses `radixconfig.yaml`, **not** `docker-compose.yaml`. 


## Built With

* [.NET](https://www.microsoft.com/net)
* [Docker](https://www.docker.com/) - Containerization

