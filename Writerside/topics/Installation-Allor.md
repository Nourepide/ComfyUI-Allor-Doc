# Installation Allor

Once **ComfyUI** is installed, you won't have any trouble augmenting it with the **Allor** plugin.

### By Manager

If you have [ComfyUI-Manager](https://github.com/ltdrdata/ComfyUI-Manager) installed, you can install Allor by manager.

### By Download

<tabs group="installing">
<tab title="Installation for Unix" group-key="unix">

<procedure>

1. **Download Allor**: Download
   the [Allor ZIP archive](https://github.com/Nourepide/ComfyUI-Allor/archive/refs/heads/main.zip).
2. **Unzip the Archive**: Unzip the downloaded archive to the `ComfyUI/custom_nodes` directory.
3. **Run the Installation Script**: Execute the `install.sh` file. You can do this from the terminal with the following
   command:

    ```bash
    bash install.sh
    ```
4. **Run ComfyUI**: Finally, run ComfyUI.

</procedure>

</tab>
<tab title="Installation for Windows" group-key="windows">

<procedure>

1. **Download Allor**: Download
   the [Allor ZIP archive](https://github.com/Nourepide/ComfyUI-Allor/archive/refs/heads/main.zip).

2. **Unzip the Archive**: Unzip the downloaded archive to the `ComfyUI\custom_nodes` directory.

3. **Run the Installation Script**: Execute the `install.bat` file. You can do this from the command prompt with the
   following command or just click on it:

    ```bash
    install.bat
    ```

4. **Run ComfyUI**: Finally, run ComfyUI.

</procedure>

</tab>
</tabs>

### With Git

<tabs group="installing">
<tab title="Installation for Unix" group-key="unix">

<procedure>

See how to [Work with Terminal](Work-with-Terminal.md).

1. **Open Terminal**: Navigate to the `ComfyUI/custom_nodes` directory.

2. **Clone the Repository**: Clone the repository by entering the following command:

    ```bash
    git clone https://github.com/Nourepide/ComfyUI-Allor.git
    ```

3. **Navigate to the Allor Folder**: Enter the Allor folder using the following command:

    ```bash
    cd ComfyUI-Allor
    ```

4. **Run the Installation Script**: Execute the `install.bat` script by entering the following command:

    ```bash
    bash install.sh
    ```

5. **Run ComfyUI**: Finally, run ComfyUI.

</procedure>

</tab>
<tab title="Installation for Windows" group-key="windows">

<procedure>

See how to [Work with Terminal](Work-with-Terminal.md).

1. **Open Command Prompt**: Navigate to the `ComfyUI\custom_nodes` folder.

2. **Clone the Repository**: Clone the repository by entering the following command:

    ```bash
    git clone https://github.com/Nourepide/ComfyUI-Allor.git
    ```

3. **Navigate to the Allor Folder**: Enter the Allor folder using the following command:

    ```bash
    cd ComfyUI-Allor
    ```

4. **Run the Installation Script**: Execute the `install.bat` script by entering the following command:

    ```bash
    install.bat
    ```

5. **Run ComfyUI**: Finally, run ComfyUI.

</procedure>

</tab>
</tabs>

## What does the installation script do?

1. **Searches for the virtual environment**: The script checks for a Python virtual environment.

2. **Installs dependencies**: If a `requirements.txt` file exists in the current directory, the script installs the
   dependencies listed in it.

3. **Initializes a Git repository**: If Git is installed and the current directory is not yet a Git repository, the
   script initializes a new Git repository and syncs it with a remote repository.

4. **Uses GitPython**: If Git is not installed, the script uses GitPython, a Python library, to perform Git operations.

5. **Finishes its work**: Finally, the script deactivates the Python virtual environment.
