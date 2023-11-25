# Modules

In Allor, **modules** are integral components that are loaded into the **ComfyUI**, containing **nodes** that users
interact with.

This page provides detailed information about each module, helping you understand their **functionality**.

In Allor, **modules** have the flexibility to utilize various **implementations** as a backend for nodes.
This versatility allows for a diverse range of **functionalities** and **interactions** within the plugin.

Here is a backend list:

* **PyTorch** — Image processing with Tensor without transformation.
* **NumPy** — PyTorch and NumPy arrays share their underlying memory locations, allowing for efficient transformations without any performance loss.
* **OpenCV** — An open-source library dedicated to real-time image processing. It offers even higher operation speeds than pure tensor processing.
* **Pillow** — A widely used Python library for image manipulation. Slow speed of work, if possible, we will switch from it to OpenCV.
* **Rembg** — A specialized library for removing image backgrounds. Despite its slower operation speed (up to 30 seconds), it provides effective background removal capabilities.

### Alpha Chanel

Module for working with **transparency** chanel in images. Allows you to create, add, restore or remove alpha chanel.

**Backend**: PyTorch.

### Image Container

Module that allows you to create an **empty container** based on the images
for use as **size value** and **mathematical operations** with it.

**Backend**: PyTorch.

### Image Composite

Module that allows you to **place images** of different sizes on top of **each other** while maintaining transparency.

**Backend**: PyTorch.

### Image Segmentation

Module for **removing background** from images.
For the better result, it is recommended to add prompt that generates plain background.

**Backend**: Rembg.

### Image Text

Module that allows you to **create text as image**.
In the future will be moved to Image Draw module.

**Backend**: Pillow.

### Image Draw

Module for **draw figures** as images.
This module may be reworked in the future.

**Backend**: Pillow.

### Image Effects

Module for working with **visual effects** and **optical distortions**.

**Backend**: OpenCV, PyTorch.

### Image Filter

A module for changing the image by **applying mathematical operations**.
Unlike effects, it does not focus on artwork changes.

**Backend**: Pillow.

### Image Noise

Module for working with noise on images. In early stage of development.

**Backend**: NumPy.

### Image Transform

Module for **changing the representation** of images.
Allows you to resize, reflect, expand, rotate and crop images.

**Backend**: PyTorch, Pillow.

### Image Batch

Module for comfortable work with **batch image processing**.
Allows adding images to batch, splitting, removing or getting the desired image from the array.

**Backend**: PyTorch.

### Clamp

The module that provides a **strongly typed solution** to improve the **readability of nodes**.

The nodes within this module uniquely have their module name positioned at the end of their name,
rather than at the beginning.

**Backend**: PyTorch.
