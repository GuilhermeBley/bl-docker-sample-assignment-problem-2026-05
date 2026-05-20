# Dockerize BOTH apps - the Python and the Node app.

## 1) Create appropriate images for both apps (two separate images!).
Go to `assignment-problem\node-app\Dockerfile` path in the terminal
Type `docker build -t bl-sample-2026-05-my-node-app .` (create the image)
Then `docker run -p 3000:3000 bl-sample-2026-05-my-node-app` (run the container)

## 2) Launch a container for each created image, making sure, that the app inside the container works correctly and is usable.

## 3) Re-create both containers and assign names to both containers. Use these names to stop and restart both containers.

## 4) Clean up (remove) all stopped (and running) containers, clean up all created images.

## 5) Re-build the images - this time with names and tags assigned to them.

## 6) Run new containers based on the re-built images, ensuring that the containers are removed automatically when stopped.