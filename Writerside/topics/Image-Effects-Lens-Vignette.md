# Vignette

<deflist type="narrow">
    <def title="Full Name">
        ImageEffectsLensVignette
    </def>
    <def title="Description">
        Apply a camera lens decreasing in the brightness and saturation to the images.
    </def>
        <def title="Backend">
            <a href="Modules.md" anchor="pytorch" summary="Image processing with pure Tensor without transformations.">PyTorch</a>
        </def>
    <def title="Input Parameters">
        <deflist type="narrow">
            <def title="Images">
                RGB/A images
            </def>
            <def title="Lens Shape">
                Form of lens
            </def>
            <def title="Lens Edge">
                If around is selected, the lens will adjust to the proportions of the image
            </def>
            <def title="Lens Curvy">
                The value of the curve during the propagation of the effect, where 1.0 is linear
            </def>
            <def title="Lens Zoom">
                How close lens are to the center of images
            </def>
            <def title="Brightness">
                Adjust brightness of images with a scale.
            </def>
            <def title="Saturation">
                Adjust color saturation of an images with a scale
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
