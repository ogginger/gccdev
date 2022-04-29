This is a containerized gcc development environment that is intended to be used with vscode.

To develop using this environment, you will need to install the following software:
    1. vscode
        a. remote - containers extension
    2. docker

To get started:
    1. Enter your git email address into the .devcontainer/devcontainer.json file.
    2. Enter the name of the project into the CMakeLists.txt file.
    3. Press F1 and type/select "Remote-Containers: Rebuild and Open in Container."
    4. Press the button in the bottom right to configure cmake tools.
        a. Select the gcc kit from the dropdown menu when prompted.
        b. Select whether to automatically configure cmake tools when opening the directory.


