# Celestial Bodies Database

A database of the universe, built with **PostgreSQL**: galaxies, stars, planets, moons and constellations, all connected to each other.

## In plain words

I designed and built a relational database from scratch, organizing information about space into **five related tables** (`galaxy`, `star`, `planet`, `moon` and `constellation`). Each star belongs to a galaxy, each planet orbits a star and each moon orbits a planet, and the tables are linked so the data stays organized and consistent.

This project is the result of my own effort and a key part of my learning. I built it step by step, working through each requirement and learning how relational databases are designed as I went.

> This is a guided learning project from the freeCodeCamp **Relational Databases** certification. The requirements and environment come from freeCodeCamp; the database is my own implementation.

## Skills this project shows

- **Database design:** organizing information into related tables with primary keys and foreign keys
- **Data organization:** keeping data consistent across connected tables
- **PostgreSQL:** creating a database and saving it as a file that can be restored
- **Tools:** Git, VS Code and Docker dev containers
- **Learning mindset:** completing a structured certification project from start to finish

## What's in this repository

| File | Description |
| --- | --- |
| `universe.sql` | The finished database (tables, relationships and data), ready to restore |

## How to run it

You need PostgreSQL installed. To restore the database:

```bash
psql -U postgres < universe.sql
```

To open it:

```bash
psql -U postgres -d universe
```

## Prerequisites

1. [Docker Engine](https://docs.docker.com/engine/)
2. [VS Code](https://code.visualstudio.com/download) and the [Dev Containers](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers) extension
3. Git

### How to Run a Project in Docker

1. Clone the RDB Alpha repo with `git clone https://github.com/freeCodeCamp/rdb-alpha`
2. Open a terminal, navigate to the `rdb-alpha` directory, and open VSCode with `code .`
3. Press Ctrl / Cmd + Shift + P and enter `Dev Containers: Rebuild Container and Reopen in Container`
4. A new VS Code window will open and begin building the Docker image. It will take several minutes to build the first time.
5. Once the image is finished building, press Ctrl / Cmd + Shift + P and enter `CodeRoad: Start` to open CodeRoad
6. In the CodeRoad window, click "Start New Tutorial"
7. Enter the URL to the `tutorial.json` file of the project you want to start (ex: https://raw.githubusercontent.com/freeCodeCamp/learn-bash-by-building-a-boilerplate/main/tutorial.json)
8. Click the "Start" button

There may be some additional troubleshooting steps to get the container running properly. They can often be solved by following the onscreen instructions, or examining any error messages in your terminal.

### How to Restart or Switch Projects

Note: If you restart or switch projects you will lose your progress, along with any files or directories you created.

1. Press Ctrl / Cmd + Shift + P and enter `Dev Containers: Rebuild Container`
2. Wait for VS Code to reopen and reload the Docker container
3. Open CodeRoad, enter the URL to a `tutorial.json` file, and start the project as described above

### `tutorial.json` File URLs for CodeRoad

* [Celestial Bodies Database](https://raw.githubusercontent.com/freeCodeCamp/learn-celestial-bodies-database/main/tutorial.json)

## Credits

Original environment and tutorial by [freeCodeCamp](https://github.com/freeCodeCamp/rdb-alpha).
