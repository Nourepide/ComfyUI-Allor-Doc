# Adjustment

<deflist type="narrow">
    <def title="Full Name">
        ImageEffectsAdjustment
    </def>
    <def title="Description">
        Corrects the color and light characteristics of images.
    </def>
        <def title="Backend">
            <a href="Modules.md" anchor="pytorch" summary="Image processing with pure Tensor without transformations.">PyTorch</a>
        </def>
    <def title="Input Parameters">
        <deflist type="narrow">
            <def title="Images">
                RGB/A images
            </def>
            <def title="Brightness">
                Determines the degree of the pixel illumination in the image
            </def>
            <def title="Contrast">
                Controls the difference between the lightest and darkest parts of the image
            </def>
            <def title="Saturation">
                Controls the intensity of the colors in the image
            </def>
            <def title="HUE">
                Allows you to change the color gamut of an image by shifting all colors by a certain number of degrees
                on the color wheel
            </def>
            <def title="Gamma">
                Changes the brightness of the image, but retains the black and white tones
            </def>
            <def title="Sharpness">
                Increases or decreases the clarity of an image by increasing or softening borders and details
            </def>
            <def title="Red">
                Controls the intensity of the red color in the image
            </def>
            <def title="Green">
                Controls the intensity of the green color in the image
            </def>
            <def title="Blue">
                Controls the intensity of the blue color in the image
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
