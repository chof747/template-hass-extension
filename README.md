# Template project for home assistant custom component development projects

This project is a boilerplate template for custom components development in home assistant
which is prepared to run also additional services (like an mqtt broker)

This project includes already:

- The vscode configuration for a dev container
- The container definition inside a docker-compose file
- A stub for a custom component

## Install

1. Copy the repository to any place convenient
2. Rename the project from sensorinterface to the real name
3. Adjust the following lines in the docker-compose file to meet the name of your project:
```yaml
    volumes:
      - .:/workspaces/sensorinterface
```
4. Adjust the following line in the .devcontainer/devcontainer.json file:
```json
	"workspaceFolder": "/workspaces/sensorinterface",
```