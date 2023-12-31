# Installation ComfyUI
Before installing **Allor**, you need to have **Python** and **ComfyUI** installed.

### How to get ComfyUI

<procedure>

For **Windows** systems, you can [download portable version](https://github.com/comfyanonymous/ComfyUI/releases/download/latest/ComfyUI_windows_portable_nvidia_cu121_or_cpu.7z) and go straight to the [Allor installation](Installation-Allor.md) step.

Also, you can get **ComfyUI** from a [direct download](https://github.com/comfyanonymous/ComfyUI/archive/refs/heads/master.zip) link.

And finally, you can get **ComfyUI** using [Git](https://git-scm.com/) by typing this command into the terminal.
```Bash
git clone https://github.com/comfyanonymous/ComfyUI.git
```

</procedure>

### How to get Python

<tabs group="installing">
<tab title="Python for Unix" group-key="unix">

<procedure>

**Python** comes **preinstalled** on most **Linux** distributions, and is available as a package on all others.

* You can check if **Python** is installed on your system from the terminal with the following command:

    ```bash
    python3 --version
    ```
If **Python** is not installed on your system, you can also install it via the terminal.

* For **Arch Linux**

    ```bash
    pacman -S python
    ```

* For **macOS** with [Homebrew](https://brew.sh/)
    ```bash
    brew install python
    ```

On **macOS**, you can also download the **Python** installer from the [official site](https://www.python.org/downloads/).

</procedure>

</tab>
<tab title="Python for Windows" group-key="windows">

<procedure>

On **Windows** systems, you can get **Python** in a number of ways.

* The easiest way to install **Python** for **Windows** is to download it from the [official site](https://www.python.org/downloads/).

* You can also install **Python** using the [Microsoft Store](https://apps.microsoft.com/detail/9NRWMJP3717K).

* Through **Powershell** you can install it by [Windows Package Manager](https://learn.microsoft.com/en-us/windows/package-manager/winget/).
   ```bash
   winget install python
   ```

* And finally, you will be able to install **Python** through the terminal using [Chocolatey](https://chocolatey.org/).
    ```bash
    choco install python
   ```

After installation, you need to verify that **Python** is running correctly.

* Open the **terminal** and type this command:
    ```bash
    python3 --version
    ```

You can do this by pressing <shortcut>Win+R</shortcut> and typing `cmd`.

</procedure>

</tab>
</tabs>

### Setup Python Environment

Of course, you can skip this step and go straight to installing the dependencies, but I still **recommend** you create a **virtual environment** specifically for **ComfyUI**.

This will allow you to create an **isolated space** that has its **own independent set** of installed **Python packages**.

This will prevent a system **pollution**, eliminate **dependency conflicts**, and exclude the possibility of other **projects affecting** the operation of **ComfyUI**.

<tabs group="installing">
<tab title="Setup for Unix" group-key="unix">

<procedure>

See how to [Work with Terminal](Work-with-Terminal.md).

1. **Open Terminal**: Navigate to the `ComfyUI` root directory.

2. **Create Virtual Environment**: You can do it by typing the following command.
    ```Bash
   python -m venv
    ```

3. **Activate new Environment**: You can do this by writing this command to your terminal.
    ```Bash
   source venv/bin/activate
    ```

</procedure>

</tab>
<tab title="Setup for Windows" group-key="windows">

<procedure>

See how to [Work with Terminal](Work-with-Terminal.md).

1. **Open Command Prompt**: Navigate to the `ComfyUI` root folder.

2. **Create Virtual Environment**: You can do it by typing the following command.
    ```Bash
   python -m venv
    ```

3. **Activate new Environment**: You can do this by writing this command to your terminal.
    ```Bash
   .\venv\Scripts\activate
   ```

</procedure>

</tab>
</tabs>

After activating the **virtual environment**, all commands applicable to **Python** will be intercepted.
This means that they will use the **Python version** from the **virtual environment**, not the system version.

It's also worth noting that the **Python version** in the **virtual environment** may differ from the system one, as well as the installed packages.

If you need to return to the system **Python** version and **exit** the **virtual environment**, enter this command:
```Bash
deactivate
```

### Install Dependencies

One of the most important steps in installing **ComfyUI** is installing **dependencies**.

**Dependencies** are external **modules** or **libraries** that **ComfyUI** uses to perform its functions.

<tabs group="installing">
<tab title="Dependencies for Unix" group-key="unix">

<procedure>

See how to [Work with Terminal](Work-with-Terminal.md).

1. **Open Terminal**: Navigate to the `ComfyUI` root directory.

2. **Install PyTorch Dependencies**:
    * **For AMD**:
        ```Bash
        pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/rocm5.6
        ```

    * **For NVIDIA**:
        ```Bash
        pip install torch torchvision torchaudio --extra-index-url https://download.pytorch.org/whl/cu121
        ```

    * **For Apple Mac silicon**:
      ```Bash
      pip install --pre torch torchvision torchaudio --extra-index-url https://download.pytorch.org/whl/nightly/cpu
      ```

3. **Install ComfyUI Dependencies**: You can install it by typing the following command.
   ```Bash
   pip install -r requirements.txt
   ```


</procedure>

</tab>
<tab title="Dependencies for Windows" group-key="windows">

<procedure>

See how to [Work with Terminal](Work-with-Terminal.md).

1. **Open Command Prompt**: Navigate to the `ComfyUI` root folder.

2. **Install PyTorch Dependencies**:
    * **For AMD**:
        ```Bash
        pip install torch-directml
        ```

    * **For NVIDIA**:
        ```Bash
        pip install torch torchvision torchaudio --extra-index-url https://download.pytorch.org/whl/cu121
        ```

3. **Install ComfyUI Dependencies**: You can install it by typing the following command.
   ```Bash
   pip install -r requirements.txt
   ```

</procedure>

</tab>
</tabs>

### Run ComfyUI

The hardest part is behind, now you can launch **ComfyUI** and start generating your first images.

<tabs group="installing">
<tab title="Run on Unix" group-key="unix">

<procedure>

See how to [Work with Terminal](Work-with-Terminal.md).

1. **Type into Terminal**: Now you can finally run **ComfyUI** by following command.
    * **Run on Linux**:
        ```Bash
        python main.py
        ```

    * **Run on macOS**:
      ```Bash
      python main.py --force-fp16
      ```

2. For your **convenience**, you can create a bash **script**, such as a `run.sh` file, to avoid manually activating the
   **virtual environment** and running **ComfyUI** from the terminal each time you want to use it.

    ```Bash
    #!/bin/bash

    source venv/bin/activate

    if [[ "$OSTYPE" == "linux-gnu"* ]]; then
        python main.py
    elif [[ "$OSTYPE" == "darwin"* ]]; then
        python main.py --force-fp16
    fi
    ```

3. After creating a **script** file, you can run it by command:

    ```Bash
    bash run.sh
    ```

</procedure>

</tab>
<tab title="Run on Windows" group-key="windows">

<procedure>

See how to [Work with Terminal](Work-with-Terminal.md).

1. **Open Command Prompt**: Now you can finally run **ComfyUI** by following command.
    * **Run on AMD**:
        ```Bash
        python main.py --directml
        ```

    * **Run on NVIDIA**:
        ```Bash
        python main.py
        ```

2. For your convenience, you can create a **script**, such as a `run.bat` file, to avoid manually activating the
   **virtual environment** and running **ComfyUI** from the terminal each time you want to use it.

<tabs>
<tab title="Script for NVIDIA">

```Bash
@echo off
call .\venv\Scripts\activate
python main.py
```

</tab>
<tab title="Script for AMD">

```Bash
@echo off
call .\venv\Scripts\activate
python main.py --directml
```

</tab>
</tabs>

</procedure>
</tab>
</tabs>

After launching **ComfyUI**, it will be accessible at the local address [127.0.0.1:8188](http://127.0.0.1:8188/) in your **browser**.
