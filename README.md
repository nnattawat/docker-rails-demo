# Running app with docker
Make sure you have installed Docker native then run the following commands
```
# build images
docker-compose build

# Setup db
docker-compose run app bundle exec rake db:create
docker-compose run app bundle exec rake db:migrate

# Run rails server using CMD in Dockerfile
docker-compose up

# Running test
docker-compose run app bundle exec rake test
```

# Todo
- [ ] build on CI and push image up to ECR
- [ ] Deploy onto ECS
