# dockter

Docker containers can produce more logs than a terminal is comfortable handling. dockter collects container output, stores it in one place, and lets you search and filter the stored logs through a desktop interface.

## Features

- Collect live container logs through the Docker Engine API.
- Store container logs in MongoDB.
- Search stored logs for relevant entries.
- Filter logs to narrow the data shown in the interface.

## Installation

Before installing dockter, make sure Docker is installed with at least one running container, MongoDB is available, and Yarn is installed.

Clone the repository and install its dependencies:

```sh
git clone <repository-url> dockter
cd dockter
yarn
```

Build the TypeScript application when needed:

```sh
yarn build
```

## Usage

Start dockter from the project directory:

```sh
yarn start
```

With Docker and MongoDB running, dockter connects to the Docker Engine, collects available container logs, and provides search and filter controls for the stored data.

For local development, use:

```sh
yarn dev
```

## License

MIT License. dockter is based on [oslabs-beta/Dockter](https://github.com/oslabs-beta/Dockter), which is also licensed under the MIT License. See the `LICENSE` file for the full license text and attribution requirements.
