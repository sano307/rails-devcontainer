# rails-devcontainer

How to link Rails and VSCode Remote Container.

## Requirements

- [Docker Compose](https://docs.docker.com/compose/install/)
- [VSCode Remote Container](https://code.visualstudio.com/docs/remote/containers/)

## Environment

- macOS (Catalina)

## Usage

Open the VSCode, and then just press `command + shift + p`, select the `Remote-Containers: Reopen in Container`.

Next, you have to create a new terminal on the VSCode screen, some like below.

```sh
vscode ➜ /workspace (main) $
```

Lastly, run `rails s` and open the browser to `http://localhost:3000`

```sh
$ rails s
```
