# VS Code Customization Repository

This repository holds all the settings, custom CSS, and JavaScript files I use to personalize my Visual Studio Code experience.

## Features

* **Settings Extensions:** [Listed here](./extensions.md)
* **Custom CSS:** Improve the look and feel of your code editor with custom styles.
* **Custom JavaScript:** Add additional functionality to VS Code through custom scripts.

## Installation

There are two ways to use these customizations in your VS Code environment:

**1. Using the "Custom CSS and JS Loader" extension:**

1. Install the "Custom CSS and JS Loader" extension from the VS Code Marketplace.
2. Copy the following settings to your VS Code User Settings (Code > Preferences > Settings):

```json
{
  "vscode_custom_css.imports": [
     "path/to/your/custom.css" // Replace with the path to your custom CSS file
     "path/to/your/custom.js" // Replace with the path to your custom JS file (optional)
  ],
}
```

* Make sure the paths in the settings point to the actual locations of your CSS and JS files within this repository (relative paths work).
* Enable "Custom CSS and JS Loader" from the VS Code command palette (Ctrl+Shift+P or Cmd+Shift+P on macOS).
* After making changes to your CSS or JS files, use the "Reload Custom CSS and JS" command in the command palette to see the updated styles and functionality.

**2. Manual Integration:**

1. Copy the desired settings files (e.g., settings.json) from this repository to your VS Code User Settings directory. The location can be found by opening the settings editor (Code > Preferences > Settings) and clicking on "Open Settings (JSON)" at the bottom left corner.
2. Copy your custom CSS and JS files to a convenient location within your VS Code workspace or user profile.
3. Update the relevant VS Code settings (e.g., `markdown.styles`) to point to the location of your custom CSS file.

**Note:** When using the "Custom CSS and JS Loader" extension, it's recommended to disable conflicting settings from other extensions that might affect the loaded styles and scripts.
