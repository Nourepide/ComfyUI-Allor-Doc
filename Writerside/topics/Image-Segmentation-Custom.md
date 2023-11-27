# Custom

<deflist type="narrow">
    <def title="Full Name">
        ImageSegmentationCustom
    </def>
    <def title="Description">
        Removes background from images with an outer model.
    </def>
        <def title="Backend">
            <a href="Modules.md" anchor="rembg" summary="A specialized library for removing image backgrounds.">Rembg</a>
        </def>
    <def title="Input Parameters">
        <deflist type="narrow">
            <def title="Images">
                RGB/A images
            </def>
            <def title="Model">
                Image segmentation model from ONNX folder
            </def>
            <def title="Alpha Matting">
                Alpha matting is a post-processing step that can be used to improve the quality of the output
            </def>
            <def title="Alpha Matting Foreground Threshold">
                Trimap foreground threshold
            </def>
            <def title="Alpha Matting Background Threshold">
                Trimap background threshold
            </def>
            <def title="Alpha Matting Erode Size">
                How far will the transparency spread from the original mask
            </def>
            <def title="Post-Process Mask">
                Post-processing mask, makes it rougher
            </def>
            <def title="Mean">
                Clarifying value
            </def>
            <def title="Std">
                The divisor of the final value
            </def>
            <def title="Size">
                Title size. Different models support different sizes. Or their multiple values [512 -> 1024 -> 2048...]
            </def>
        </deflist>
    </def>
    <def title="Output Parameters">
        <deflist type="narrow">
            <def title="Images">
                RGB/A images
            </def>
        </deflist>
    </def>
</deflist>
