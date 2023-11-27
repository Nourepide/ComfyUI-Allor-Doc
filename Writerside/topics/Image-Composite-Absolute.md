# Absolute

<deflist type="narrow">
    <def title="Full Name">
        ImageCompositeAbsolute
    </def>
    <def title="Description">
        Places images on top of each other in a virtual container with pixel accuracy.
    </def>
        <def title="Backend">
            <a href="Modules.md" anchor="pytorch" summary="Image processing with pure Tensor without transformations.">PyTorch</a>
        </def>
    <def title="Input Parameters">
        <deflist type="narrow">
            <def title="Images A">
                RGB/A images
            </def>
            <def title="Images B">
                RGB/A images
            </def>
            <def title="Images A X">
                First images horizontal position in container from left to right
            </def>
            <def title="Images A Y">
                First images vertical position in container from top to bottom
            </def>
            <def title="Images B X">
                Second images horizontal position in container from left to right
            </def>
            <def title="Images B Y">
                Second images vertical position in container from top to bottom
            </def>
            <def title="Container Width">
                The width of the container in which the images will be placed, if 0 are defined automatically
            </def>
            <def title="Container Height">
                The height of the container in which the images will be placed, if 0 are defined automatically
            </def>
            <def title="Background">
                What images will be placed on the background
            </def>
            <def title="Method">
                <list>
                    <li><control>Pair</control> — The images from the batches will be merged according to the sequence number.</li>
                    <li><control>Matrix</control> — The image from the batches will be merged with all images.</li>
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
