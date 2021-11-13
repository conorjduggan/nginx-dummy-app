# nginx-dummy-app

Implementation of a dummy nginx app for use in projects

## Building
1. Move back up a directory, outside of the project dir.
    * `cd ../`
2. Package the Helm project.
    * `helm package nginx-dummy-app`

## Deploying manually
1. If you haven't already done so from the previous section, move back up a directory, outside of the project dir.
    * `cd ../`
2. Install the Helm package.
    * `helm install nginx-dummy-app nginx-dummy-app`

## Deploying using argocd
Please follow the steps outlined in [Deploying nginx-dummy-app using argocd](https://github.com/conorjduggan/argocd#deploying-nginx-dummy-app-using-argocd).