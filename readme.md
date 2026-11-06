# mcman

A lightweight, interactive Minecraft server manager built in Go.

## Features

- Interactive terminal interface powered by `go-choice`
- First-time setup wizard for fresh installations or existing servers
- Direct server JAR installer for **Paper** and **Purpur** with version pickers and live download progress
- Automatic discovery of server folders and `.jar` files
- Persistent configuration stored in `mcman.json`
- Built-in memory allocation presets
- Aikar's optimized G1GC JVM flags toggle
- Automatic EULA acceptance (`eula.txt`)
- Direct interactive console passthrough for server commands

## Requirements

- Go 1.20+
- Java Runtime Environment (matching your Minecraft version, e.g. Java 17 or Java 21)

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

### First-Time Setup Wizard

If no `mcman.json` is found on launch, the wizard prompts you to:
1. Download a fresh server JAR (Paper / Purpur) or connect to an existing server folder.
2. Select your target directory (`./server`, `./`, or a custom path).
3. Select the Minecraft version to download.
4. Set RAM allocation and toggle Aikar's JVM performance flags.

### Main Menu

- **Start Server**: Boots the Minecraft server using the saved configuration and attaches the terminal to the server console.
- **Download / Install Server JAR**: Fetch and download any Paper or Purpur version at any time.
- **Settings & Configuration**: Modify your server directory, JAR selection, memory allocation, and JVM arguments.
- **Exit**: Close the manager.

### Configuration (`mcman.json`)

Settings are stored in `mcman.json` next to the executable:

```json
{
  "server_dir": "./server",
  "jar_file": "paper-1.21.4-232.jar",
  "ram": "4G",
  "use_aikar": true,
  "nogui": true,
  "extra_flags": []
}
```

## License

MIT
