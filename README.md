# Face Detection Project with TensorJS

This project uses TensorJS for face detection. It includes a web application with face detection capabilities using the camera.

## Project Structure

- `docker-compose.yaml`: Docker Compose file for setting up the project environment.
- `Dockerfile`: Dockerfile for building the project image.
- `index.html`: Main HTML file for the web application.
- `package.json`: Node.js package configuration.
- `slim-dockerfile`: Slim Dockerfile for a smaller project image.
- `src/`:
  - `camera.js`: Module for camera-related functionality.
  - `index.js`: Main entry point for the web application.
  - `option_panel.js`: Module for handling options panel.
  - `shared/`:
    - `option_panel.js`: Shared option panel functionality.
    - `params.js`: Parameters module.
    - `stats_panel.js`: Module for displaying statistical information.
    - `util.js`: Utility functions.

### Quick Demo
```
docker run -p 1234:1234 harshmanvar/face-detection-tensorjs:slim-v1
```
Open URL in browser

`http://localhost:1234`

<img width="832" alt="Screenshot 2023-08-02 at 1 23 45 AM" src="https://github.com/harsh4870/face-detection-tensorjs/assets/15871000/a32b6ad6-2a69-4119-9506-50f2dd1a0198">

### Getting Started

![image1](https://github.com/harsh4870/face-detection-tensorjs/assets/15871000/33f9f879-04f2-45ea-8499-c1d91dcff956)

#### Building the Image

```
docker build  -t tensor-development:v1 .
```

#### Running  the Container

```
docker run -p 1234:1234 -v $(pwd):/app -v /app/node_modules tensor-development:v1 watch
```

Open URL in browser

`http://localhost:1234`

#### Monitoring container with Docker Desktop

<img width="727" alt="image4" src="https://github.com/harsh4870/face-detection-tensorjs/assets/15871000/c86003c5-435c-41ea-86b9-35b53b69bf94">
