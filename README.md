# rosana-cli

The **rosana-cli** tool is a command-line utility that helps you quickly set up projects using the **Rosana.js** framework. It automates the creation and updating of Rosana-based applications, providing an easy-to-use interface for developers.

With **rosana-cli**, you can generate a new project with a recommended structure, complete with example patterns, and update an existing project.

## Features

- **Create a New Project**: Generate a new Rosana-based app with a predefined structure.
- **Update Existing Projects**: Update dependencies and project files to keep them in sync with the latest Rosana framework standards.
- **Open in VSCode**: Optionally open the project in Visual Studio Code after creation or update.

---

## Installation

You can install **rosana-cli** globally on your machine for easy access. To install it globally, run:

```bash
npm install -g rosana-cli
```

This will make the `rs` command available from anywhere on your system.

---

## Usage

### `rs create <project-name>`

Creates a new project based on the **Rosana.js** framework. The CLI will automatically generate a new project folder with the recommended directory structure, example files, and basic configurations.

#### Arguments:

- `<project-name>`: The name of the new project you want to create.

#### Example:

```bash
rs create my-new-app
```

This will create a new folder called `my-new-app` in the current directory with the basic structure and necessary configuration files to start building with the **Rosana.js** framework.

#### Options:

- `--open`: Optionally open the newly created project in Visual Studio Code.

#### Example:

```bash
rs create my-new-app --open
```

This command will create the app and then attempt to open it in VSCode (if VSCode is installed and available in the system path).

---

### `rs update`

Updates an existing Rosana-based project to the latest version of the framework, ensuring that dependencies and project files are up to date.

#### Example:

```bash
rs update
```

This will update the project’s dependencies and configurations to the latest recommended versions of **Rosana.js**.

---

## Files and Directories Created

When you use `rs create`, the following structure will be set up for you:

```bash
my-new-app/
  ├── .pages
  │   ├── .ui/
  │       ├── buttons.js
  │       └── navigation.js
  │   ├── index,js
  │   └── about.js
  ├── .src/
  │   ├── public/
  │   ├── styles/
  │   └── scripts
  ├── node_modules/
  ├── package.json
  ├── index.html
  ├── App.js
  └── vite.config.js
```

- **app/**: Contains the main application files, including the entry point (`index.js`), component definitions, and styles.
- **node_modules/**: Automatically created after you install dependencies with npm.
- **package.json**: The configuration file for your Node.js project, including dependencies, scripts, and metadata.
- **vite.config.js**: Vite configuration for bundling the project.

---

## Development

To start the project in development mode after creation:

1. Navigate into the project folder:

    ```bash
    cd my-new-app
    ```

2. Install dependencies:

    ```bash
    npm install
    ```

3. Start the development server:

    ```bash
    npm run dev
    ```

This will launch the Vite development server and open your app in the browser.

---

## License

The **rosana-cli** tool is open-source and available under the MIT License.

---

## Contributing

If you would like to contribute to the development of **rosana-cli**, feel free to fork the repository, make your changes, and submit a pull request.
