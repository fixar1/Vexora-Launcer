# Vexora-Launcer

Vexora Launcher

A modern Minecraft: Java Edition launcher for Windows.

Vexora Launcher is an independent desktop application designed to make managing Minecraft installations, mod loaders, mods, and modpacks easier. It combines a modern interface with isolated game instances and built-in download management.

Features

* Multiple game instances — create, copy, rename, configure, and remove separate Minecraft installations.
* Minecraft versions — browse releases, snapshots, and older versions.
* Mod loaders — support for Vanilla, Fabric, Quilt, Forge, and NeoForge, subject to version compatibility.
* Modrinth integration — search for mods, manage versions and dependencies, and import or export .mrpack modpacks.
* Java management — detect installed Java versions and download compatible Mojang-provided Java runtimes.
* Download manager — progress tracking, cancellation, retries, and file integrity checks.
* Microsoft account authentication — intended for users who own Minecraft: Java Edition and are eligible to access Minecraft services.
* Offline mode — launch compatible offline or offline-mode servers using a local username.
* Local storage — keep instances, settings, and game files organized on the user’s computer.
* Modern interface — a dark-themed UI with animations and a responsive layout.

Technology Stack

* Electron
* React
* TypeScript
* Vite
* Tailwind CSS
* Framer Motion
* SQLite
* Zod

Requirements

* Windows 10 or Windows 11
* Node.js 22 or later for development
* A Microsoft account and a valid Minecraft: Java Edition entitlement for licensed online play

Development

Clone the repository and install dependencies:

git clone https://github.com/YOUR-USERNAME/vexora-launcher.git
cd vexora-launcher
npm install

Start the development environment:

npm run dev

Run checks:

npm run typecheck
npm test

Build the Windows installer:

npm run dist

The generated installer is placed in the release directory.

Microsoft Authentication

Vexora Launcher is designed to use Microsoft authentication followed by the Xbox and Minecraft authentication services.

Microsoft authentication requires an application registration and a configured Client ID. Access to Minecraft services must also comply with Microsoft’s and Mojang’s applicable requirements and approval process.

Live Microsoft, Xbox, and Minecraft authentication must be verified separately. A successful Microsoft sign-in alone does not guarantee access to Minecraft services.

Vexora Launcher does not provide Minecraft licenses or bypass ownership checks.

Privacy and Security

* Microsoft passwords are entered through the authentication flow rather than requested directly by the launcher.
* Authentication tokens are intended to be stored securely using operating-system facilities.
* Sensitive tokens should not be included in logs or public source code.
* Never commit .env files, credentials, access tokens, or other private configuration to the repository.

Project Status

Vexora Launcher is under active development.

Core launcher features have automated tests, but live authentication, downloads from official game services, mod-loader installation, and end-to-end gameplay still require verification on supported Windows systems.

Features and compatibility may change as development continues.

Disclaimer

Vexora Launcher is an independent community project and is not affiliated with, endorsed by, or sponsored by Microsoft or Mojang Studios.

Minecraft is a trademark of Mojang Studios. All respective trademarks belong to their owners.
