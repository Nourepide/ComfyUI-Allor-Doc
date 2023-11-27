# Resize Clip

<deflist type="narrow">
    <def title="Full Name">
        ImageTransformResizeClip
    </def>
    <def title="Description">
        Resizes the image to the limits specified in the parameters while preserving the aspect ratio.
    </def>
        <def title="Backend">
            <a href="Modules.md" anchor="pytorch" summary="Image processing with pure Tensor without transformations.">PyTorch</a>
        </def>
    <def title="Input Parameters">
        <deflist type="narrow">
            <def title="Images">
                RGB/A images
            </def>
            <def title="Max Width">
                Maximum allowable image width in pixels
            </def>
            <def title="Max Height">
                Maximum allowable image height in pixels
            </def>
            <def title="Min Width">
                Minimum allowable image width in pixels
            </def>
            <def title="Min Height">
                Minimum allowable image height in pixels
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
