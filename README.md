# Resin .NET Core Hello World
A simple `Hello, World!` application that demonstrates the use of multi-stage builds to deploy a standalone .NET Core 2.0 application to a Resin device.

## Requirements
* `git`
* [Resin.io account](https://dashboard.resin.io/signup) 
* [Resin.io application](https://docs.resin.io/management/applications/)
* A [provisioned device](https://docs.resin.io/management/devices/)

## Deployment
1. Clone this repository
2. Add the Resin `git` endpoint:
````
git remote add resin <username>@git.resin.io:<username>/<application_name>.git
````
The full endpoint can also be found in the application screen on the [dashboard](https://dashboard.resin.io/apps).

3. Initiate a multi-stage deployment:
````
git push resin master:resin-emulated
````
__NOTE__: This deployment process is slightly different from the normal process. See [this blog post](https://resin.io/blog/multi-stage-docker-builds-for-tiny-iot-images/) for more details.
