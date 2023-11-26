# Configuration

**Allor** can be configured using the `config.json` file. This file is created during the **first launch** of Allor,
based on the template found in `template/template.json`.

In the event of an **update**, the configuration file **automatically adapts** to all changes. It **preserves old
parameters** while removing outdated ones and applying new ones. This ensures that your configuration stays
**up to date** with the latest features and improvements.

## Modules

In this section, you have the ability to **disable** any modules that you do not need to load. By default, all modules
are **enabled** (set to `true`).

| Name              | Type    | Default | Description                                      |
|-------------------|---------|---------|--------------------------------------------------|
| AlphaChanel       | Boolean | True    | Manages the transparency of images.              |
| Clamp             | Boolean | True    | Manage nodes for readability.                    |
| ImageBatch        | Boolean | True    | Handles batch image processing.                  |
| ImageComposite    | Boolean | True    | Combines multiple images into one.               |
| ImageContainer    | Boolean | True    | Get images size as container.                    |
| ImageDraw         | Boolean | True    | Draws shapes onto images.                        |
| ImageEffects      | Boolean | True    | Applies various effects to images.               |
| ImageFilter       | Boolean | True    | Filters images using different algorithms.       |
| ImageNoise        | Boolean | True    | Adds or reduces noise in images.                 |
| ImageSegmentation | Boolean | True    | Divides an image background.                     |
| ImageText         | Boolean | True    | Create text as images.                           |
| ImageTransform    | Boolean | True    | Transforms images by rotating, scaling, and etc. |

## Override

With **Allor**, you have the flexibility to **disable** the standard nodes of ComfyUI that have similar functionality
available in Allor. By default, all overrides are **disabled** (set to `false`).

<table>
<thead>
  <tr>
    <th>Name</th>
    <th>Type</th>
    <th>Default</th>
    <th>Original</th>
    <th>New</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td rowspan="10">postprocessing</td>
    <td rowspan="10">Boolean</td>
    <td rowspan="10">False</td>
    <td>ImageBlend</td>
    <td>-</td>
  </tr>
  <tr>
    <td rowspan="7">ImageBlur</td>
    <td>ImageFilterBlur</td>
  </tr>
  <tr>
    <td>ImageFilterBoxBlur</td>
  </tr>
  <tr>
    <td>ImageFilterGaussianBlur</td>
  </tr>
  <tr>
    <td>ImageFilterGaussianBlurAdvanced</td>
  </tr>
  <tr>
    <td>ImageFilterStackBlur</td>
  </tr>
  <tr>
    <td>ImageFilterMedianBlur</td>
  </tr>
  <tr>
    <td>ImageFilterBilateralBlur</td>
  </tr>
  <tr>
    <td>ImageQuantize</td>
    <td>-</td>
  </tr>
  <tr>
    <td>ImageSharpen</td>
    <td>-</td>
  </tr>
  <tr>
    <td rowspan="4">transform</td>
    <td rowspan="4">Boolean</td>
    <td rowspan="4">False</td>
    <td>ImageScale</td>
    <td>ImageTransformResizeAbsolute</td>
  </tr>
  <tr>
    <td>ImageScaleBy</td>
    <td>ImageTransformResizeRelative</td>
  </tr>
  <tr>
    <td rowspan="2">ImageInvert</td>
    <td>ImageTransformRotate</td>
  </tr>
  <tr>
    <td>ImageTransformTranspose</td>
  </tr>
  <tr>
    <td rowspan="7">debug</td>
    <td rowspan="7">Boolean</td>
    <td rowspan="7">False</td>
    <td>LatentBlend</td>
    <td>-</td>
  </tr>
  <tr>
    <td>LoadLatent</td>
    <td>-</td>
  </tr>
  <tr>
    <td>SaveLatent</td>
    <td>-</td>
  </tr>
  <tr>
    <td>TomePatchModel</td>
    <td>-</td>
  </tr>
  <tr>
    <td>FreeU</td>
    <td>-</td>
  </tr>
  <tr>
    <td>FreeU_V2</td>
    <td>-</td>
  </tr>
  <tr>
    <td>HyperTile</td>
    <td>-</td>
  </tr>
</tbody>
</table>

## Updates

In this section, you can **configure the auto-update feature** of Allor or even **disable it** entirely.

| Name                      | Type    | Default | Description                                                                                    |
|---------------------------|---------|---------|------------------------------------------------------------------------------------------------|
| update_frequency          | String  | day     | Sets how often Allor should check for updates. Available - Always, Never, Day, Week and Month. |
| notify_if_has_new_updates | Boolean | True    | Notify you when new updates are available                                                      |
| notify_if_no_new_updates  | Boolean | True    | Notify you when there are no new updates.                                                      |
| auto_update               | Boolean | True    | Automatically update itself if update available.                                               |
| branch_name               | String  | main    | Specifies the branch that Allor should pull updates from.                                      |
| update_mode               | String  | soft    | Determines how indifferent the update will be to inconsistencies. Available - Soft, Hard.      |

## Fonts

Some nodes require fonts to function. In this section, you can configure where **Allor** should look for these fonts.

| Name         | Type    | Default            | Description                                                                                             |
|--------------|---------|--------------------|---------------------------------------------------------------------------------------------------------|
| folder_path  | String  | comfy_extras/fonts | Specifies the path where Allor should look for fonts. You can use `\` or `/` symbol for path splitting. |
| system_fonts | Boolean | False              | Use the system’s fonts.                                                                                 |
| user_fonts   | Boolean | False              | Use the user's fonts. Doesn't affect on Windows because all fonts contains in system folder.            |
