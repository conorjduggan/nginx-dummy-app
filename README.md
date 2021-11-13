# nginx-dummy-app

Implementation of a dummy nginx app for use in projects.

I have just wrapped the official nginx Docker image into my own Docker image, for the purposes of being able to build, push, and pull a Docker image as part of CI/CD testing.

## Building the Docker image
1. `docker build -t cduggan123/nginx-dummy-app:1.14.2`

## Publishing the Docker image to Docker Hub
1. `docker push cduggan123/nginx-dummy-app:1.14.2`

## Building the Helm artifact
1. Move back up a directory, outside of the project dir.
    * `cd ../`
2. Package the Helm project.
    * `helm package nginx-dummy-app`

## Deploying the Helm artifact manually
1. If you haven't already done so from the previous section, move back up a directory, outside of the project dir.
    * `cd ../`
2. Install the Helm package.
    * `helm install nginx-dummy-app nginx-dummy-app`

## Deploying  the Helm artifact using argocd
Please follow the steps outlined in [Deploying nginx-dummy-app using argocd](https://github.com/conorjduggan/argocd#deploying-nginx-dummy-app-using-argocd).