docker build -t react-redux-jwt-auth:dev .

docker run \
    -it \
    --rm \
    -v ${PWD}:/app \
    -v /app/node_modules \
    -p 3001:3000 \
    -e CHOKIDAR_USEPOLLING=true \
    react-redux-jwt-auth:dev



docker build -f Dockerfile.prod -t react-redux-jwt-auth:v1 .

docker build -f Dockerfile.prod -t react-redux-jwt-auth:v1 .

docker run -it --rm -p 1337:80 react-redux-jwt-auth:v1
