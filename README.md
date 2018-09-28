# Boilerplate for nginx with Let’s Encrypt on docker-compose

This repository is accompanied by a [step-by-step guide](https://medium.com/@pentacent/nginx-and-lets-encrypt-with-docker-in-less-than-5-minutes-b4b8a60d3a71).

## Installation
1. [Install docker-compose](https://docs.docker.com/compose/install/#install-compose)

2. Clone this repository: `git clone https://github.com/wmnnd/nginx-certbot.git .`

3. Modify configuration:
- Add domains and email addresses to init-letsencrypt.sh
- Replace all occurrences of example.org with primary domain (the first one you added to init-letsencrypt.sh) in data/nginx/app.conf

4. Run init the script
```
chmod +x ./init-letsencrypt.sh
sudo ./init-letsencrypt.sh
```

5. Run server
`docker-compose up`

## Got questions?
Feel free to post questions in the comment section of the [accompanying guide](https://medium.com/@pentacent/nginx-and-lets-encrypt-with-docker-in-less-than-5-minutes-b4b8a60d3a71)

## License
All code in this repository is licensed under the terms of the `MIT License`. For further information please refer to the `LICENSE` file.