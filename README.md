# SOURCE

Please note the source of this repo is started from:

[https://github.com/knative/docs](https://github.com/knative/docs/tree/main/docs/serving/samples/hello-world/helloworld-kotlin)

Under the license of `CC BY 4.0`


## Requirements

You just need to have docker installed.

Note this project does NOT use Knative.


## Building and Running

From the root project directory,

`docker build . -t hwk`

Once the image is built successfully, you can launch it with

`docker run -d -p 8080:8080 --name hwk hwk`

You should see `hwk` at the top of your

`docker ps`

Visit [localhost:8080](http://localhost:8080) and you should see "Hello World".


## Clean Up

For clean up, you can delete the container and image:

```
docker stop hwk
docker rm hwk
docker rmi hwk
```
