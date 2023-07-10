# Local development environment for python data projects, with Docker

A simple ETL project that fetches 10 records and loads them into a postgres database representing our data warehouse.

The Purpose of this simple project is to help on setting up a local development environment for future data projects using Docker

## Pre-requisite

To run the code, you will need

1. [Docker](https://docs.docker.com/get-docker/) and [Docker Compose](https://docs.docker.com/compose/install/)(v1.27.0 or later)
2. [git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)

Clone the git repo and run the ETL as shown below.

```bash
git clone https://github.com/josephmachado/local_dev.git
cd local_dev
make up
make ci # run tests and format code
make run-etl # run the ETL process
make down # spins down the containers
```

For more details, please read the post: [Setting up local dev environment with Docker](https://www.startdataengineering.com/post/local-dev/).
