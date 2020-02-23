# Delete all containers
docker rm -vf $(docker ps -a -q)

# Delete all images
docker rmi -f $(docker images -a -q)

# Build an image (from directory containing the Dockerfile)
docker build --rm -f Dockerfile -t [name]:[tag] .

# Run the container
docker run --rm -it [name]:[tag]

# Commit container
docker commit [container_id] [name]:[tag]

# Tag image
docker tag [image_id] rafrdz/[name]:[tag]

# Push to Docker Hub
docker push rafrdz/[name]