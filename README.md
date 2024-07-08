# demo-app

This is a simple angular web app. It was generated with [Angular CLI](https://github.com/angular/angular-cli) version 17.0.8.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The application will automatically reload if you change any of the source files.

## Docker build and run

```docker build . -t demo-app
docker run -p 8080:80 -e ENVIRONMENT=Production demo-app
```
The app should be reachable on http://localhost:8080.

## Deploy to Kubernetes

 ```
 # Push the local image to an image registry

docker tag demo-app:latest <your-dockerhub-id>/demo-app:v1
docker push <your-dockerhub-id>/demo-app:v1

# Patch the image tag in manifests/deployment.yaml and run:

`kubectl apply -f manifests/
```

The app should be reachable on http://localhost:30001.
