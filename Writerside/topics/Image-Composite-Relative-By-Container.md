# Relative By Container

<deflist type="narrow">
    <def title="Full Name">
        ImageCompositeRelativeByContainer
    </def>
    <def title="Description">
        Places images on top of each other in the outer container with scale factor accuracy.
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
