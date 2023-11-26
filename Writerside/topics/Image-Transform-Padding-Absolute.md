# Padding Absolute

<deflist type="narrow">
    <def title="Full Name">
        ImageTransformPaddingAbsolute
    </def>
    <def title="Description">
        Adds new space around the edges of images by pixels.
    </def>
        <def title="Backend">
            <a href="Modules.md" anchor="pytorch" summary="Image processing with pure Tensor without transformations.">PyTorch</a>
        </def>
    <def title="Input Parameters">
        <deflist type="narrow">
            <def title="Images">
                RGB/A images
            </def>
            <def title="Add Width">
                New width in pixels on horizontal edges
            </def>
            <def title="Add Height">
                New height in pixels on vertical edges 
            </def>
            <def title="Method">
                <list>
                    <li><control>Reflect</control> — The new space reflects the images around the edges.</li>
                    <li><control>Edge</control> — The new space is filled with pixels at the edges of the image.</li>
                    <li><control>Constant</control> — The new space is filled with emptiness.</li>
                </list>
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
