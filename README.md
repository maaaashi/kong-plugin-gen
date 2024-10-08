![kong](./docs/kong.png)

# CreateKongPlugin

CreateKongPlugin is a CLI tool designed to simplify and speed up the process of generating template files for creating Kong plugins. With just a single command, developers can quickly create the necessary files and directory structure needed for Kong plugin development, allowing them to focus on coding their plugin functionality.

## Key Features
- Quick Template Generation: Instantly generate template files for Kong plugins.
- Customizable: Easily specify plugin names and directory structure to fit your project.
- Lightweight & Easy to Use: Simple commands for fast setup and development.

## Installation

To install CreateKongPlugin, simply use the go install command:

```
go install github.com/maaaashi/create-kong-plugin@latest
```

Make sure that your Go environment is properly set up and that the $GOPATH/bin directory is included in your system's PATH, so you can run the create-kong-plugin command from anywhere in your terminal.

## Usage
CreateKongPlugin is designed to be simple to use. You can generate a new Kong plugin with a single command.

```
create-kong-plugin my-plugin
```

## Available Commands
- completion: Generate the autocompletion script for the specified shell.
- help: Display help information about any command.

## Example Usage

### Create a New Plugin

To create a new Kong plugin template, simply run:

```
create-kong-plugin my-plugin
```

This will generate a folder with the following structure:

```
my-plugin/
│
├── src/
│   │
│   ├── handler.lua
│   └── schema.lua
│
└── kong-plugin-my-plugin-0.1.0-1.rockspec
```

### Generate Shell Autocompletion
You can also generate an autocompletion script for your shell:

```
create-kong-plugin completion bash
```

## Flags

- -h, --help: Show help for a specific command.
- -t, --toggle: Example flag toggle.
To get more detailed help on a specific command, run:

```
create-kong-plugin [command] --help
```

## Contributing

Feel free to submit issues, suggestions, or pull requests to the GitHub repository.

## License
CreateKongPlugin is open-source and available under the MIT License.
