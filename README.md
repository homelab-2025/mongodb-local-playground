## mongodb-local-playground

This guide will walk you through setting up a MongoDB Replicaset with dockerc-compose

### Prerequisites

- [Docker Desktop](https://www.docker.com/products/docker-desktop/) installed

### Getting started

1. Clone the repo

```bash
git clone https://github.com/homelab-2025/mongodb-local-playground.git
```

2. Once done, you can create the MongoDB Replicaset using the command:

```bash
docker-compose up -d
```

3. Then when the containers are up, you can connect to the mongodb replicaset by typing:

```bash
docker exec -it mongo1 mongosh
```

4. Finally, you can check the status of the replicaset by typing:

```bash
rs.status()
```

You should be able to see the 3 members of the replicaset with one PRIMARY  and two SECONDARY 
