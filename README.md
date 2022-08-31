# hasura-docker-compose

## Step 1

Adjust the `docker-compose.yml` file with your env variables

## Step 2

Run docker image with `docker-compose up -d`

## Step 3

Verify that the image is running with `docker ps`

It should show to containers (one for hasura's graphql engine and the other a regular postgres db):

```
CONTAINER ID IMAGE                 ... CREATED STATUS PORTS          ...
097f58433a2b hasura/graphql-engine ... 1m ago  Up 1m  8080->8080/tcp ...
b0b1aac0508d postgres              ... 1m ago  Up 1m  5432/tcp       ...
```

## Step 4

Head to http://localhost:8080/console to open the Hasura console.

Navigate to Data -> Manage -> Connect Database and set up a new database connection.
