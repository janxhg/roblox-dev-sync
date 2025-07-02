# Roblox Dev Sync

A server that allows you to sync files between Roblox Studio and your favorite IDE. Develop your Roblox games using your preferred code editor while maintaining a live connection with Roblox Studio.

## 🔌 Install the Plugin in Roblox Studio

1. **Download and Install the Plugin**

   * Go to: [https://create.roblox.com/store/asset/137634224705881/ConnectYourIDE](https://create.roblox.com/store/asset/137634224705881/ConnectYourIDE)

   * Click on `Get Plugin`

   * Open Roblox Studio and enable the plugin

   * Two plugin buttons will appear: one to **export** the project files to your IDE, and another to **sync** the changes

   * Recommended: Enable the HTTP server, click **Export**, then click **Sync**

   * Everything you save in your IDE will automatically reflect in the Roblox project

   > **Note**: If a script doesn't update in Roblox Studio, try closing and reopening the script tab to view the latest changes.



## ⚙️ Server Installation

### Requirements

* Python 3.7 or higher
* pip (Python package manager)

### Install via pip

```bash
pip install roblox-dev-sync
```



## 🚀 Start the Server

### Using the CLI

```bash
roblox-sync
```

The server will start on `http://localhost:3000` by default.



## 🛠 Usage

1. **Start the Server**

   * Open a terminal in the folder where you want to keep your Roblox project
   * Run `roblox-sync`
   * The server will initialize and show the project directory

2. **Create a New Project**

   * Open Roblox Studio
   * Create a new game or open an existing one
   * Use the plugin to export the project
   * Then click **Sync** to establish the connection

3. **Edit Files**

   * You can now edit `.lua` files directly in your IDE
   * Changes made in your IDE will automatically sync with Roblox Studio
   * Changes in Roblox Studio will also sync back to your IDE



## ⚙️ Configuration

### Project Directory

* Default: `./roblox_projects`
* You can change it by editing the `PROJECTS_DIR` variable in the code

### Server Port

* Default: `3000`
* You can change it by editing the `SYNC_PORT` variable



## ✨ Features

* Bidirectional sync between Roblox Studio and your IDE
* Supports all Roblox script types
* File watcher for real-time updates
* Automatically manages directory structure
* REST interface for communication with Roblox Studio



## 📬 Support

* Report issues via the GitHub repository
* Contact: `NetechAI@proton.me`



## 📄 License

This project is licensed under the **Apache 2.0** License. See the `LICENSE` file for more details.

