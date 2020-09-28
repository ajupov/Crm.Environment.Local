# Crm.Environment.Local

Local environment configs for [Lite CRM](https://litecrm.org)

## Usage

### Requirements

- [Docker](https://hub.docker.com/editions/community/docker-ce-desktop-windows)

### Common information

**Before pull Docker images needs login to private Docker registry**

#### Layers

1. **Services layer**: `postgres`, `redis`
2. **Backend layer**: `identity`, `apps`
3. **Frontend layer**: `site`, `account`

- You can run `Services` layer in Docker, `Backend` and `Frontend` layers in run IDE for development
- Or you can run `Services` and `Backend` layers in Docker, `Frontend` layers run in IDE for development

#### Running

1. **Services layer**: `docker-compose -f docker-compose-services.yml up`
2. **Backend layer**: `docker-compose -f docker-compose-backend.yml up`
3. **Frontend layer**: `docker-compose -f docker-compose-backend.yml up`
