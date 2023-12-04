# Updating

Maintaining the **latest version** of Allor is crucial for **optimal performance** and access to **new features**.

This section provides comprehensive instructions on how to **update Allor**, whether you prefer the convenience of
**automatic updates** or the control of **manual updates via Git**.

## Auto-Update

**Allor** has the capability to **self-update**. By default, this happens **once a day**.

If you wish to **modify this behavior** or **disable auto-update**, please refer to the <a href="Configuration.md" anchor="updates">
configuration</a> page.

### Troubleshooting  { id="troubleshooting_auto_update" }

If you have problems with auto-update, you can switch it to **hard mode** in configuration.

This will **ensure** that the repository is updated to the latest version at the cost of a **factory reset**.
This will remove any changes you may have made to the Allor code.

This **does NOT** affect ComfyUI, other plugins, last update timestamp and the Allor configuration file.

## Manual updating with Git

> You need to have Git installed.

<tabs group="updating">
<tab title="Updating for Unix" group-key="unix">

<procedure>

See how to [Work with Terminal](Work-with-Terminal.md).

1. **Open Terminal**: Navigate to the `ComfyUI/custom_nodes/ComfyUI-Allor` directory.

2. **Update the Repository**: Update the repository by entering the following command:

    ```bash
    git pull
    ```

</procedure>

</tab>
<tab title="Updating for Windows" group-key="windows">

<procedure>

See how to [Work with Terminal](Work-with-Terminal.md).

1. **Open Command Prompt**: Navigate to the `ComfyUI\custom_nodes\ComfyUI-Allor` folder.

2. **Update the Repository**: Update the repository by entering the following command:

    ```bash
    git pull
    ```

</procedure>

</tab>
</tabs>

### Troubleshooting { id="troubleshooting_git" }

As with [auto-update](Updating.md#troubleshooting_auto_update), you can reset the **Allor** repository to the latest state if you find problems.

<procedure>

1. Get the current state of the remote repository:

```Bash
git fetch origin main
```

2. Reset the current state to the remote repository level

```Bash
git reset --hard origin/main
```

</procedure>

Be **careful** when using these **commands**, as they completely **remove** all manual **changes** made by the user to **Allor**.
