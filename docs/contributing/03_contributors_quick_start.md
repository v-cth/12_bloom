# Note to Starters

TrawlWatcher is POC (Proof Of Concept) project as we write

There are two ways you can run Trawlwatch dev env:

* (Recommended) With Docker containers and a Docker Compose stack (on your local machine)
* With a local virtual environement (on your local machine). This virtual environement is
  managed via Poetry by default but you can create your own if preferred

If you want to use Docker, see pre-requisite [Docker Installation](https://docs.docker.com/get-docker/) on your machine

If you want to use a local Virtual Environment with Poetry, see [Poetry Basic Usage](https://python-poetry.org/docs/basic-usage/)

If you want to use your own Virtual Env, see [VENV package basics](https://docs.python.org/3/library/venv.html)

# Demand Access to official Trawlwatch Repository (Recommended way)

Trawlwatch is a communtary project managed by [Data For Good](https://dataforgood.fr/)

For Trawlwatch project, it has been discussed and preferred that contributors ask for repository access
to contribute as it has been considered simpler for beginner developers and for repository managers
in order to managed and update the branches if needed to integrate

You can use forks to start your work but as soon as possible, just ask access to the project team by:
* joining [Slack Channel](https://app.slack.com/client/T04GWR7E4/C06C8R4FNH1)

# Local dev with Docker/Docker Compose

## Pre-requisites

* Install [Git](https://git-scm.com/)
* Install [Docker Community Edition](https://docs.docker.com/get-docker/) with Compose plugin

## Setting development environment

* clone and enter the repository :

```
cd <your projects folder>
git clone https://github.com/dataforgoodfr/12_bloom.git
cd 12_bloom
```

* Launch the default Docker Compose stack
```
docker compose up

```
Output:
```
[+] Running 3/3
 ✔ Container postgres_bloom  Created                                                                               0.1s
 ✔ Container init_bloom      Created                                                                               0.5s
 ✔ Container bloom           Created                                                                               0.5s
Attaching to bloom, init_bloom, postgres_bloom
postgres_bloom  | The files belonging to this database system will be owned by user "postgres".
postgres_bloom  | This user must also own the server process.
postgres_bloom  |
...
bloom           |   You can now view your Streamlit app in your browser.
bloom           |
bloom           |   URL: http://0.0.0.0:8501
bloom           |
```

* Check to the application wbe browsing http://localhost:8501