docker build -f Dockerfile.dev .

docker run -p 3000:3000 <id>

docker run -p 3000:3000 -v /app/node_modules -v $(pwd):/app <id>

Old: docker run pushpit07/docker-react npm run test -- --coverage
Updated: docker run -e CI=true pushpit07/docker-react npm run test