## create react app with docker

`docker build --tag cra-docker-image:1 .`

Some of you found that your container stopped running immediately after starting. This is because react-scripts exits after start-up. We can get around this by running in interactive mode i.e. we add the option `-it`.

`docker run -it --name cra-docker-container -p 3003:3000 cra-docker-image:1`
