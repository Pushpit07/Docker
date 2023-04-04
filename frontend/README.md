docker build -f Dockerfile.dev .

docker run -p 3000:3000 <id>

docker run -p 3000:3000 -v /app/node_modules -v $(pwd):/app <id>

Old: docker run pushpit07/docker-react npm run test -- --coverage
Updated: docker run -e CI=true pushpit07/docker-react npm run test


docker-compose -f docker-compose-dev.yml up
docker-compose -f docker-compose-dev.yml up --build
docker-compose -f docker-compose-dev.yml down


Note:
https://www.udemy.com/course/docker-and-kubernetes-the-complete-guide/learn/lecture/11437142#questions/17673926