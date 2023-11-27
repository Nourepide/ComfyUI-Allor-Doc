# Inheritance Sum

<deflist type="narrow">
    <def title="Full Name">
        ImageContainerInheritanceMax
    </def>
    <def title="Description">
        Takes the size of the image and creates an empty container based on it with the size of their size's sum.
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
            <def title="Red">
                Red channel of container
            </def>
            <def title="Green">
                Green channel of container
            </def>
            <def title="Blue">
                Blue channel of container
            </def>
            <def title="Alpha">
                Alpha channel of container
            </def>
            <def title="Method">
                <list>
                    <li><control>Sum</control> — Sum width and height.</li>
                    <li><control>Sum Height</control> — Sum only height.</li>
                    <li><control>Sum Width</control> — Sum only width.</li>
                </list>
            </def>
            <def title="Method">
                <list>
                    <li><control>Single</control> — Create only one container.</li>
                    <li><control>For Each Pair</control> — Create container for each image in batch.</li>
                    <li><control>For Each Matrix</control> — Create container for each image in batch with each other.</li>
                </list>
            </def>
        </deflist>
    </def>
    <def title="Output Parameters">
        <deflist type="narrow">
            <def title="Image">
                RGB/A images
            </def>
        </deflist>
    </def>
</deflist>
