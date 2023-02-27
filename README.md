# Spryker B2C Demo Shop

### Installing the B2C Demo Shop

To install the B2C Demo Shop:

1. Create a project folder and clone the B2C Demo Shop and the Docker SDK:
```bash
mkdir spryker-b2c && cd spryker-b2c
git clone https://github.com/wesolowski/b2c-demo-shop.git ./
git clone git@github.com:spryker/docker-sdk.git docker
```

#### Setting up a development environment

To set up a development environment:

1. Bootstrap the docker setup:

```bash
docker/sdk boot deploy.dev.yml
```

Hosts file:
```bash
sudo bash -c "echo '127.0.0.1 backend-api.at.spryker.local backend-api.de.spryker.local backend-api.us.spryker.local backend-gateway.at.spryker.local backend-gateway.de.spryker.local backend-gateway.us.spryker.local backoffice.at.spryker.local backoffice.de.spryker.local backoffice.us.spryker.local date-time-configurator-example.spryker.local glue.at.spryker.local glue.de.spryker.local glue.us.spryker.local mail.spryker.local queue.spryker.local redis-commander.spryker.local scheduler.spryker.local spryker.local swagger.spryker.local yves.at.spryker.local yves.de.spryker.local yves.us.spryker.local' >> /etc/hosts"
```

2. If the command you've run in the previous step returned instructions, follow them.

3. Build and start the instance:
```bash
docker/sdk up -x
```

