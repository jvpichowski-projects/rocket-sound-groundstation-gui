# RocketSound Grundstation Gui

[![Created using the @wuespace/telestion-client-cli](https://img.shields.io/badge/created%20using-%40wuespace%2Ftelestion--client--cli-%23452897)](https://github.com/TelestionTeam/telestion-client/tree/main/packages/telestion-client-cli)

This project contains the gui for the *RocketSound Groundstation*. 
The groundstation is based on [Telestion](https://github.com/TelestionTeam) that is a modular groundstation system.

This gui project was bootstrapped with the
[Telestion Gui Client](https://github.com/TelestionTeam/telestion-client) CLI.

## Getting started

> **NOTE:** All commands below, unless otherwise specified,
> should get executed in the cloned project's root folder (that contains the `package.json`) or a subfolder thereof.

The first step is to install the development dependencies.
They are defined in `package.json` and you can install them with the following command:

```shell script
npm ci
```

## Running

To build and run the project in development mode, execute:

```shell script
npm start
```

## Build and deploy

The build command generates a ready-to-deploy web application and native app.

To build the entire project, run:

```shell script
npm run build
```

## Project structure

The project structure is like the structure created by `create-react-app` (_CRA_), plus some special structures:

```
.
├── public (static files, cf. CRA documentation)
│   ├── index.html
│   ├── favicon.ico
│   └── [...]
├── src
│   ├── components
│   │   ├── app.tsx (the overall PSC React App)
│   │   ├── header.tsx (the header component)
│   │   └── login-page.tsx (the login page)
│   ├── model
│   │   └── sample-user-config.ts (the initial user config)
│   ├── widgets
│   │   ├── sample-widget (a sample widget included in the template)
│   │   │   ├── index.ts (widget meta model, including a unique widget name)
│   │   │   └── widget.tsx (widget component definition)
│   │   └── index.ts (array of widgets)
│   ├── index.css
│   ├── index.tsx
│   └── [...]
├── package.json
├── README.md (you're here :P)
├── telestion.config.js (configuration of the PSC, such as plugins, etc.)
└── tsconfig.json (configuration for TypeScript compilation)
```

## Learn More

To get started with gui development, you can take a look at the _PSC Developer Manual_. It contains many explanations of the most important concepts, practical guides, references, and more.

You can find the latest versions (in PDF format) in the [Documentation Repo Releases](https://github.com/TelestionTeam/telestion-docs/releases/latest).

For a full API Reference of all the Telestion Gui Client APIs, check out the documentation of the Telestion Client:
https://telestionteam.github.io/telestion-client/

To learn React, check out the [React documentation](https://reactjs.org/).
