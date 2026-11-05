# mcman

A lightweight, interactive Minecraft server manager built in Go.

## Features

- Terminal UI for easier managing
- Automatic discovery of server folders and `.jar` files
- Persistent configuration stored in `mcman.json`
- Automatic EULA acceptance
- Direct console passthrough for server commands

## Requirements

- Go 1.20+
- Java Runtime Environment (matching your Minecraft version, e.g. Java 17 or Java 21, some versions even need Java 25)

## Installation

Clone the repository and build the binary:

```bash
git clone https://github.com/yourusername/mcman.git
cd mcman
go build -o mcman.exe .
```

## Usage

Run the executable in your workspace:

```bash
./mcman.exe
```

### Main Menu

- **Start Server**: Starts the Minecraft server using the saved config and attaches the terminal to the server console.
- **Setup & Flags Configuration**: Modify your server directory, JAR selection, memory allocation, and JVM arguments.
- **Exit**: Close the manager.

### Configuration (`mcman.json`)

Settings are stored in `mcman.json` next to the executable:

```json
{
  "server_dir": "./server",
  "jar_file": "server.jar",
  "ram": "4G",
  "use_aikar": true,
  "nogui": true,
  "extra_flags": []
}
```

## License

This program is licensed under the GNU General Public License v3 

