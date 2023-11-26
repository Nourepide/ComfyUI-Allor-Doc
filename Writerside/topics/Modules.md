# Modules

In Allor, **modules** are general components that are loaded into the **ComfyUI**, containing **nodes** that users
interact with.

This page provides detailed information about each module, helping you understand their **functionality**.

In Allor, **modules** have the flexibility to utilize various **implementations** as a backend for nodes.
This versatility allows for a diverse range of **functionalities** and **interactions** within the plugin.

Here is a list of backends:

<list>
<li id="pytorch">
    <control>PyTorch</control> — Image processing with pure Tensor without transformations.
</li>
<li id="numpy">
    <control>NumPy</control> — PyTorch and NumPy arrays share underlying memory locations, allowing for efficient transformations without any performance loss.
</li>
<li id="opencv">
    <control>OpenCV</control> — An open-source library dedicated to real-time image processing. It offers even higher operation speeds than pure tensor processing.
</li>
<li id="pillow">
    <control>Pillow</control> — A widely used Python library for image manipulation. Slow speed of work, if possible, we will switch from it to OpenCV.
</li>
<li id="rembg">
    <control>Rembg</control> — A specialized library for removing image backgrounds. Despite its slower operation speed (up to 30 seconds), it provides effective background removal capabilities.
</li>
</list>

### Alpha Chanel

A module for working with the **transparency** channel in images,
enabling the creation, addition, restoration, or removal of the alpha channel.

**Backend**: PyTorch.

### Image Container

This module allows the creation of an **empty container** based on images
for use as a **size value** and for **mathematical operations**.

**Backend**: PyTorch.

### Image Composite

This module enables the **placement of images** of varying sizes atop **each other**, preserving transparency.

**Backend**: PyTorch.

### Image Segmentation

A module for **removing backgrounds** from images.
For optimal results, it is recommended to add a prompt that generates a plain background.

**Backend**: Rembg.

### Image Text

This module enables the **creation of a text as an image**.
Plans include moving it to the Image Draw module.

**Backend**: Pillow.

### Image Draw

A module for **drawing figures** as images.
This module may undergo rework in the future.

**Backend**: Pillow.

### Image Effects

A module for working with **visual effects** and **optical distortions**.

**Backend**: OpenCV, PyTorch.

### Image Filter

A module for altering images by **applying mathematical operations**.
Unlike effects, it does not focus on artwork changes.

**Backend**: Pillow.

### Image Noise

A module for working with noise on images. Currently, in the early stage of development.

**Backend**: NumPy.

### Image Transform

A module for **changing the representation** of images.
It enables resizing, reflecting, expanding, rotating, and cropping images.

**Backend**: PyTorch, Pillow.

### Image Batch

A module for comfortable work with **batch image processing**.
It allows adding images to a batch, splitting, removing, or getting the desired image from the array.

**Backend**: PyTorch.

### Clamp

The module provides a **strongly typed solution** to improve the **readability of nodes**.

The nodes within this module uniquely have their module name positioned at the end of their name,
rather than at the beginning.

**Backend**: PyTorch.
