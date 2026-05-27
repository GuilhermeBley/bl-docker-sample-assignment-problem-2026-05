# Dockerize BOTH apps - the Python and the Node app.
Execute all the commands in the root path.

## 1- Create appropriate images for both apps (two separate images!).

- Node project
Type `docker build -t bl-sample-2026-05-my-node-app ./assignment-problem/node-app` (create the image)

- Python project
Type `docker build -t bl-sample-2026-05-my-python-app ./assignment-problem/python-app` (create the image)

## 2- Launch a container for each created image, making sure, that the app inside the container works correctly and is usable.

- Node project
Type `docker run -p 3000:3000 bl-sample-2026-05-my-node-app` (run the container)

- Python project
Type `docker run -p 3000:3000 bl-sample-2026-05-my-python-app`

## 3- Re-create both containers and assign names to both containers. Use these names to stop and restart both containers.

- Node project
Type `docker create --name renamed-container-bl-sample-2026-05-my-node-app -p 3000:3000 bl-sample-2026-05-my-node-app`

- Python project
Type `docker create --name renamed-container-bl-sample-2026-05-my-python-app -p 3000:3000 bl-sample-2026-05-my-node-app`

## 4- Clean up (remove) all stopped (and running) containers, clean up all created images.

- Node project
`docker rm renamed-container-bl-sample-2026-05-my-node-app`

- Python project
`docker rm renamed-container-bl-sample-2026-05-my-python-app`