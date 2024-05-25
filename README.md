# Python Virtual Environment and pip

## pip: Preferred Installer Program

pip is installed by default with Python. When you install Python, you receive pip with it.

### Introduction Commands

- **Install a package:**

    ```bash
    pip install <package_name>
    ```

    or

    ```bash
    python -m pip install <package_name>
    ```

    `-m` stands for module. Both commands allow us to install a new package.

- **List installed packages:**

    ```bash
    pip list
    ```

    or

    ```bash
    python -m pip list
    ```

    This is used to list the modules that are installed in the environment along with their versions.

    Note: If `pip <command>` does not work, you must try `python -m pip <command>`. From now on, only the pip versions will be written.

- **Install a specific version of a package:**

    ```bash
    pip install <package_name>==<version>
    ```

- **Update a package:**

    ```bash
    pip install -U <package_name>
    ```

    `-U` command allows you to update the specified package.

- **Uninstall a package:**

    ```bash
    pip uninstall <package_name>
    ```

    This command allows you to delete the specified package from the environment.

## Virtual Environments

- **Create a virtual environment:**

    ```bash
    pip venv <virtual_environment_name>
    ```

    This command allows you to create an environment with the specified name.

- **Activate the environment:**

    ```bash
    source .<environment_name>/Scripts/activate
    ```

    Activates the environment which is located in the project.

- **Deactivate the environment:**

    ```bash
    deactivate
    ```

    Deactivates the environment.

- **Freeze installed packages:**

    ```bash
    pip freeze > requirements.txt
    ```

    Creates a `.txt` file, and it includes the packages that are installed in the environment along with their versions.

## .gitignore file

In order to upload the project to GitHub, the `<env_name>` directory must be ignored to avoid unnecessary storage issues.

