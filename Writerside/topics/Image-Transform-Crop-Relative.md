# Crop Relative

<deflist type="narrow">
    <def title="Full Name">
        ImageTransformCropRelative
    </def>
    <def title="Description">
        Crops images to a specified rectangular area defined by four values ranging from 0.0 to 1.0,
        where 0.0 represents the start of the image, and 1.0 represents the end of the image.
    </def>
        <def title="Backend">
            <a href="Modules.md" anchor="pytorch" summary="Image processing with pure Tensor without transformations.">PyTorch</a>
        </def>
    <def title="Input Parameters">
        <deflist type="narrow">
            <def title="Images">
                RGB/A images
            </def>
            <def title="Start X">
                Horizontal position of the initial rectangular corner in scale factor
            </def>
            <def title="Start Y">
                Vertical position of the initial rectangular corner in scale factor
            </def>
            <def title="End X">
                Horizontal position of the end rectangular corner in scale factor
            </def>
            <def title="End Y">
                Vertical position of the end rectangular corner in scale factor
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
