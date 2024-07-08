# Build

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 17.0.8.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The application will automatically reload if you change any of the source files.

## Docker build and run

For build and run:

`docker build . -t demo-app`  
`docker run -p 8080:80 -e ENVIRONMENT=Production demo-app`

 ## Run in Kubernetes

`kubectl apply -f manifests/`
