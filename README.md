# TechoramaRecap2024

## Prerequisites
Ensure that your docker engine or rancher is running on your machine.

## Getting Started
In order to create containers, you should use the following command:

```dotnet publish -t:PublishContainer```

You can change the parameters inside the project to create different containers.
Containers to create
- Create container using Ubuntu container family
- Create container using Alpine container family
- Create container using Ubuntu container family with chiseled image
- Create container with runtime identifier and self-contained image

To show your containers you created in the commandline, use the following command:

```docker images -f reference=my-api*```

## Cleanup afterwards
To cleanup all the images you created during the demo, use the following command:

```
docker rmi my-api-jammy
docker rmi my-api-alpine
docker rmi my-api-jammy-chiseled
```