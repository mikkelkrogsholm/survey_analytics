LimeSurvey
==========

LimeSurvey - the most popular
Free Open Source Software survey tool on the web.

https://www.limesurvey.org/en/

### Postgres
The repository contains a Docker Compose configuration which builds LimeSurvey with a separate Postgres-container.

**Warning**: The *docker-compose.yml* contains default PostgreSQL database credentials. It is highly recommended to change these in a production environment.

You can start the containers by running: `docker-compose up -d`

1. Go to a browser and type http://localhost
2. Click Next until you reach the *Database configuration* screen
3. Then enter the following in the field:
  - **Database type** `PostgreSQL`
  - **Database location** `pgsql`
  - **Database user** `postgres`
  - **Database password** `limesurvey`
  - **Database name** `limesurvey` # Or whatever you like
  - **Table prefix** `lime_` # Or whatever you like


### To do

#### Analytical tools
- Rstudio Server (rocker/tidyverse:3.6.0)
- Jupyter Notebook (jupyter/datascience-notebook:2ce7c06a61a1) (https://jupyter-docker-stacks.readthedocs.io/en/latest/index.html)

#### Visualization tools
- Metabase (metabase/metabase)
