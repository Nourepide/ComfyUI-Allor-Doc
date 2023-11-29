# Updating

Maintaining the **latest version** of Allor is crucial for **optimal performance** and access to **new features**.

This section provides comprehensive instructions on how to **update Allor**, whether you prefer the convenience of
**automatic updates** or the control of **manual updates via Git**.

## Auto-Update

**Allor** has the capability to **self-update**. By default, this happens **once a day**.

If you wish to **modify this behavior** or **disable auto-update**, please refer to the <a href="Configuration.md" anchor="updates">
configuration</a> page.

### Troubleshooting

If you have problems with auto-update, you can switch it to **hard mode** in configuration.

This will **ensure** that the repository is updated to the latest version at the cost of a **factory reset**.
This will remove any changes you may have made to the Allor code.

This **does NOT** affect ComfyUI, other plugins, last update timestamp and the Allor configuration file.

## Manual updating with Git

> You need to have Git installed.

<tabs group="updating">
<tab title="Updating for Unix" group-key="unix">

<procedure>

1. **Open Terminal**: Navigate to the `ComfyUI/custom_nodes/ComfyUI-Allor` directory.
 
   You can do this by opening the Terminal and using the `cd` command.

2. **Update the Repository**: Update the repository by entering the following command:

    ```bash
    git pull
    ```

</procedure>

</tab>
<tab title="Updating for Windows" group-key="windows">

<procedure>

1. **Open Command Prompt**: Navigate to the `ComfyUI\custom_nodes\ComfyUI-Allor` folder.

   You can do this by pressing <shortcut>Win+R</shortcut> and typing `cmd`.

   To change the drive, type the letter of the desired drive followed by a colon.
   For example, `D:` will switch you to the D drive.

   To move to another folder, use the cd command followed by the folder path.
   For example, `cd ComfyUI` will take you to the ComfyUI folder.

2. **Update the Repository**: Update the repository by entering the following command:

    ```bash
    git pull
    ```

</procedure>

</tab>
</tabs>
