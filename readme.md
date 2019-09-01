Survey analytics
==========

## Introduction
The goal of this repository is to create a dockerized setup, where you can collect surveys, store the data in a database and query that database using different analytical and visualization tools. 

One such setup could look like this:

`LimeSurvey` -- `Postgres` -- `Rstudio` 



Steps to get started:

1. You can start the containers by running: `docker-compose up -d`
2. Go to a browser and type http://localhost 
3. When you reach the *Database configuration* screen, then enter the following in the field:
  - **Database type** `PostgreSQL`
  - **Database location** `pgsql`
  - **Database user** `postgres`
  - **Database password** `limesurvey`
  - **Database name** `limesurvey` # Or whatever you like
  - **Table prefix** `lime_` # Or whatever you like


### LimeSurvey
LimeSurvey - the most popular Free Open Source Software survey tool on the web. (https://www.limesurvey.org/en/)

You can read the documentation here: [https://manual.limesurvey.org/](https://manual.limesurvey.org/)


### Postgres
The repository contains a Docker Compose configuration which builds LimeSurvey with a separate Postgres-container.

You can read the documentation here: [https://www.postgresql.org/docs/10/index.html](https://www.postgresql.org/docs/10/index.html)


----

### To do

#### Analytical tools
- Rstudio Server (rocker/tidyverse:3.6.0)
- Jupyter Notebook (jupyter/datascience-notebook:2ce7c06a61a1) (https://jupyter-docker-stacks.readthedocs.io/en/latest/index.html)

#### Visualization tools
- Metabase (metabase/metabase)
