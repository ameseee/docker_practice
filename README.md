# Docker Practice for Amy & Sal

How to get this app running in a container on your machine:

```
git clone git@github.com:ameseee/docker_practice.git
```

Create an image of the current repo:

```
docker-compose build
```

Spin up a container using that image:

```
docker-compose up 
```


After running those commands, open a new tab in your terminal and set up your database:

```
docker-compose run web rake db:create
docker-compose run web rake db:migrate
docker-compose run web rake db:seed
```

Visit `0.0.0.0:3000` in the browser.

