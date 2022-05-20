This is a containerized gcc development environment that is intended to be used with vscode.

To develop using this environment, you will need to install the following software:
    1. vscode: https://code.visualstudio.com/download
        a. remote - containers extension
    2. docker-ce

To get started:
    1. Enter your git email address into the .devcontainer/devcontainer.json file.
    2. Enter the name of the project into the CMakeLists.txt file.
    3. Enter the name of the project into the 'name' property located in the vcpkg.json file.
    4. Press F1 and type/select "Remote-Containers: Rebuild and Open in Container."
    5. Press the button located in the popup that appears in the bottom right to configure cmake tools.
        a. Select the gcc kit from the dropdown menu when prompted.
        b. Select whether to automatically configure cmake tools when opening the directory.
    6. Press F1 and type/select CMake: Build.

