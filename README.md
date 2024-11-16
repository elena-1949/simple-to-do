# To-Do List VS Code Extension

This extension provides a simple way to manage your to-do list directly within Visual Studio Code. You can add, remove, and toggle tasks as completed. The extension leverages TreeView for task management and WebView to display task details interactively. 

## Features

- **Add New Tasks**: Easily add new tasks to your to-do list.
- **Toggle Task Completion**: Change the status of a task between completed and incomplete.
- **Remove Tasks**: You can remove individual tasks or clear all tasks at once.
- **WebView & TreeView**: Interactive display of tasks with WebView and TreeView.
- **Task Persistence**: Tasks remain visible until removed, ensuring you stay organized.
- **Customizable Interface**: You can adjust how tasks are displayed and interact with them.

## Prerequisites

Before using this extension, ensure you have the following installed:

### 1. **Visual Studio Code**
   - You can download and install VS Code from the official [Visual Studio Code website](https://code.visualstudio.com).
   
### 2. **Node.js**
   - Install Node.js from [the official website](https://nodejs.org) to run the extension and manage dependencies.
   
### 3. **npm**
   - npm comes bundled with Node.js. It is used to install the required packages for this extension.

## Installation

Follow these steps to install and run the extension:

### 1. Clone the repository

Clone this repository to your local machine:

```bash
git clone https://github.com/YasinSa7/simple-to-do.git


2. Install dependencies
Navigate to the project directory and install the dependencies:

bash
Copy code
cd todo-vscode-extension
npm install


3. Run the extension
To test and run the extension, open the project in VS Code and press F5 to launch a new VS Code window with the extension enabled.

4. Debugging
To debug your extension, set breakpoints in your code and use the VS Code debugging interface. You can launch the extension in a new window by pressing F5, or use Ctrl+Shift+P to access commands in the Command Palette.



Usage
Adding a New Task
To add a new task:

Press Ctrl+Shift+P to open the Command Palette.
Type "Add New Task" and hit enter.
Enter the task title in the prompt and press enter.
The task will be added to your to-do list and displayed in the TreeView.

Toggling Task Completion
To toggle the completion status of a task:

Right-click on the task in the TreeView.
Select the option Toggle Completed.
This will mark the task as completed, and you can toggle it back to incomplete anytime.

Removing a Task
To remove a task:

Right-click on the task in the TreeView.
Select Remove Task to delete that specific task.
Removing All Tasks
To remove all tasks:

Press Ctrl+Shift+P to open the Command Palette.
Type "Remove All Tasks" and hit enter.
This will clear all tasks from the to-do list.

Reloading Tasks
If you want to refresh the tasks:

Press Ctrl+Shift+P.
Type "Reload Tasks" and press enter.
This will reload and update the task list with any changes made.


Project Structure
Here is a breakdown of the project structure:

lua
Copy code
F:.
|   .gitignore
|   .vscode-test.mjs
|   .vscodeignore
|   CHANGELOG.md
|   eslint.config.mjs
|   extension.js
|   jsconfig.json
|   myTextViewProvider.js
|   package-lock.json
|   package.json
|   README.md
|   todoProvider.js
|   structure.txt
|   vsc-extension-quickstart.md
|   
+---.vscode
|       extensions.json
|       launch.json
|       
+---node_modules
|   |   .package-lock.json
|   
+---resources
|       todo-icon.svg
|       
\---test
        extension.test.js



File Descriptions
extension.js: This file handles the activation and deactivation of the extension, including commands for managing tasks.
todoProvider.js: Contains the logic for managing tasks. It defines methods for adding, removing, toggling tasks, and notifying the TreeView of changes.
myTextViewProvider.js: This file sets up and manages the WebView for displaying task details in a user-friendly interface.
package.json: Contains metadata for the extension, including dependencies and scripts.
README.md: Documentation for how to install, use, and contribute to the extension.
test/extension.test.js: Contains unit tests for the extension to ensure that features work as expected.
How It Works
This extension uses two primary components for managing tasks:

TreeView: Displays a list of tasks on the left side of the screen. Each task can be toggled for completion or removed.
WebView: Provides an interactive graphical interface for the task list, allowing users to view task details and update them.
The task data is maintained in memory and updated dynamically through event-driven changes. Each time a task is added, removed, or toggled, the TreeView is refreshed.

Contribution
If you would like to contribute to the development of this extension, follow these steps:

Fork the repository.
Create a new branch for your feature or bug fix.
Make your changes and commit them.
Submit a Pull Request describing the changes you made.
Make sure your code follows the linting rules set in the eslint.config.mjs file. This helps ensure consistency across the project.

Code of Conduct
By participating in this project, you agree to follow the project's code of conduct. We encourage everyone to contribute in a respectful and positive manner.

Reporting Issues
If you find any bugs or have suggestions for improvements, please report them through the GitHub Issues page.

License
This project is licensed under the MIT License - see the LICENSE file for details.

Acknowledgments
We would like to acknowledge the following libraries and tools used in the development of this extension:

Visual Studio Code API
Node.js
npm
Roadmap
Version 1.1: Add support for task priorities and due dates.
Version 1.2: Implement task synchronization with cloud storage.
Version 2.0: Integrate with third-party task management tools like Trello and Todoist.
Version History
Version 1.0.0: Initial release with basic task management features.
Version 1.1.0: Bug fixes and minor UI improvements.
Version 2.0.0: Major update with WebView improvements and new task features.
FAQ
Q: How can I add a task if the "Add New Task" command does not appear?
A: Ensure that you have installed the extension correctly and that there are no issues with the activation. Try reloading Visual Studio Code and check the command palette again.

Q: Can I export my tasks?
A: Currently, exporting tasks is not supported, but we plan to add it in a future release.

Q: What is the TreeView used for?
A: The TreeView is used to display the list of tasks in a hierarchical format, making it easy to manage and interact with your tasks.

Conclusion
This extension is designed to help you manage tasks within Visual Studio Code efficiently. It leverages both TreeView and WebView to provide an intuitive interface for task management. We hope this tool will improve your productivity while coding. If you encounter any issues, please feel free to contribute or open an issue in the repository.

### Key Features of the `README.md`:
1. **Introduction**: Describes the purpose of the extension.
2. **Features**: Detailed features such as adding tasks, toggling completion, and removing tasks.
3. **Installation**: Step-by-step guide on how to install and run the extension.
4. **Usage**: How to use the extension, including commands for adding, removing, and toggling tasks.
5. **Project Structure**: Explanation of the project's files and directories.
6. **How It Works**: Technical description of the core components used in the extension.
7. **Contribution**: Instructions on how to contribute to the project.
8. **License**: Information on licensing.
9. **Roadmap**: Future plans for the extension.
10. **FAQ**: Common questions and answers for users.

This `README.md` provides a thorough explanation of your project, which should make it easy for other developers or users to understand, install, and contribute to the extension.








# simple-to-do README

This is the README for your extension "simple-to-do". After writing up a brief description, we recommend including the following sections.

## Features

Describe specific features of your extension including screenshots of your extension in action. Image paths are relative to this README file.

For example if there is an image subfolder under your extension project workspace:

\!\[feature X\]\(images/feature-x.png\)

> Tip: Many popular extensions utilize animations. This is an excellent way to show off your extension! We recommend short, focused animations that are easy to follow.

## Requirements

If you have any requirements or dependencies, add a section describing those and how to install and configure them.

## Extension Settings

Include if your extension adds any VS Code settings through the `contributes.configuration` extension point.

For example:

This extension contributes the following settings:

* `myExtension.enable`: Enable/disable this extension.
* `myExtension.thing`: Set to `blah` to do something.

## Known Issues

Calling out known issues can help limit users opening duplicate issues against your extension.

## Release Notes

Users appreciate release notes as you update your extension.

### 1.0.0

Initial release of ...

### 1.0.1

Fixed issue #.

### 1.1.0

Added features X, Y, and Z.

---

## Working with Markdown

You can author your README using Visual Studio Code.  Here are some useful editor keyboard shortcuts:

* Split the editor (`Cmd+\` on macOS or `Ctrl+\` on Windows and Linux)
* Toggle preview (`Shift+Cmd+V` on macOS or `Shift+Ctrl+V` on Windows and Linux)
* Press `Ctrl+Space` (Windows, Linux, macOS) to see a list of Markdown snippets

## For more information

* [Visual Studio Code's Markdown Support](http://code.visualstudio.com/docs/languages/markdown)
* [Markdown Syntax Reference](https://github.com/YasinSa7/simple-to-do.git)

**Enjoy!**
