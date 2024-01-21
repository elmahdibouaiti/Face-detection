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

