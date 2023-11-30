# Work with Terminal

At many stages with the installation of **ComfyUI** and **Allor** you will have to interact with the **terminal**
frequently, here you can learn how to use it.

If you are not yet familiar with the terminal or have never used it, you should realize one thing.

A **terminal** is simply a program that allows users to interact with a system using text commands. And a system is primarily a set of files.

For your convenience, you can think of it as a **file manager**.

<tabs group="installing">
<tab title="Unix Terminal" group-key="unix">

<procedure>

On **Unix** systems, opening a **terminal** can vary greatly depending on the **graphical environment** and the default packages supplied in the **distributions**.

* **macOS**: Pressing <shortcut>Cmd + Space</shortcut> opens **Spotlight Search**, where you can start typing `Terminal` and press <shortcut>Enter</shortcut>.
* **KDE**: Pressing <shortcut>Alt + F2</shortcut> opens the **Run Command** dialog where you can type `konsole` and press <shortcut>Enter</shortcut>.
* **Gnome**: Pressing <shortcut>Alt + F2</shortcut> opens the **Run Command** dialog where you can type `gnome-terminal` and press <shortcut>Enter</shortcut>.
* **Linux**: In most Linux graphical environments, pressing <shortcut>Ctrl + Alt + T</shortcut> will open the default terminal.

But as a rule, this does not cause any difficulty.

</procedure>

</tab>
<tab title="Windows Command Prompt" group-key="windows">

<procedure>

On **Windows** systems, you can open the **Command Prompt** in several ways. The **last two** are **preferred**.

- **With Start menu**: Click the **Start** button, then start typing `cmd` or **Command line**.

- **With Run dialog**: Press the <shortcut>Win+R</shortcut> key combination to open the **Run** dialog. Type `cmd` and press <shortcut>Enter</shortcut>.

- **With Explorer**: Navigate to the folder you need, then type `cmd` in the address bar and press <shortcut>Enter</shortcut>. This will open the command line with the current directory set to the folder you selected.

- **With context menu**: In **Explorer**, you can <shortcut>Right-Click + Shift</shortcut> and select <shortcut>Open command window here</shortcut> or <shortcut>Open PowerShell window here</shortcut> (depending on the version of Windows).

Also, you do not need to run the terminal with administrator rights during the installation of **ComfyUI** or **Allor**.

</procedure>

</tab>
</tabs>

Now it's time to learn a few little commands that we will be working with when installing **ComfyUI** and **Allor**.

<tabs group="installing">
<tab title="Unix Terminal" group-key="unix">

<procedure>

<deflist>
  <def title="pwd">
    Show you your current directory
  </def>
  <def title="ls">
    Show all files and directories in current place
  </def>
  <def title="cd dir_name">
    Change directory to <control>dir_name</control> 
  </def>
  <def title="cd ..">
    Change directory to <control>upper level</control> 
  </def>
  <def title="Pressing Tab">
    Autocomplete, such as <control>Com -> ComfyUI_windows_portable</control>
  </def>
</deflist>

</procedure>

</tab>
<tab title="Windows Command Prompt" group-key="windows">

<procedure>

<deflist>
  <def title="cd">
    Show you your current directory
  </def>
  <def title="dir">
    Show all files and directories in current place
  </def>
  <def title="A:">
    Change current disk to A
  </def>
  <def title="cd dir_name">
    Change directory to <control>dir_name</control> 
  </def>
  <def title="cd ..">
    Change directory to <control>upper level</control> 
  </def>
  <def title="Pressing Tab">
    Autocomplete, such as <control>Com -> ComfyUI_windows_portable</control>
  </def>
</deflist>

</procedure>

</tab>
</tabs>

And a couple more commands that you probably won't need during installation, but will be useful to know.

<tabs group="installing">
<tab title="Unix Terminal" group-key="unix">

<procedure>

<deflist>
  <def title="mkdir dir_name">
    Create a new directory <control>dir_name</control> 
  </def>
  <def title="rm file_name">
    Remove file <control>file_name</control> 
  </def>
  <def title="rm -r dir_name">
    Remove directory <control>dir_name</control> 
  </def>
  <def title="mv file_name new_file_name">
    Rename file or directory from <control>file_name</control> to <control>new_file_name</control> 
  </def>
  <def title="mv file_name ..\file_name">
    Move file or directory from current place to upper 
  </def>
</deflist>

</procedure>

</tab>
<tab title="Windows Command Prompt" group-key="windows">

<procedure>

<deflist>
  <def title="mkdir dir_name">
    Create a new directory <control>dir_name</control> 
  </def>
  <def title="rm file_name">
    Remove file <control>file_name</control> 
  </def>
  <def title="rd \s dir_name">
    Remove directory <control>dir_name</control> 
  </def>
  <def title="ren file_name new_file_name">
    Rename file or directory from <control>file_name</control> to <control>new_file_name</control> 
  </def>
  <def title="move file_name ..\">
    Move file or directory from current place to upper 
  </def>
</deflist>

</procedure>

</tab>
</tabs>
