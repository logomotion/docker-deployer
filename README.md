inspired by https://github.com/herloct/docker-deployer and https://github.com/buildkite/docker-ssh-env-config

## Usage
```
docker run -i --rm \
    -v /local/path:/project \
    -e SSH_PRIVATE_RSA_KEY="$(< ~/.ssh/id_rsa)" -e SSH_KNOWN_HOSTS="$(< ~/.ssh/known_hosts)" \
    logomotion/deployer deploy
```
