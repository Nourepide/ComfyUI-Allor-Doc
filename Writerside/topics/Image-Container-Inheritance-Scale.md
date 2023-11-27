# Inheritance Scale

<deflist type="narrow">
    <def title="Full Name">
        ImageContainerInheritanceScale
    </def>
    <def title="Description">
        Takes the image size and creates an empty container based on it, with the option to scale the size manually.
    </def>
        <def title="Backend">
            <a href="Modules.md" anchor="pytorch" summary="Image processing with pure Tensor without transformations.">PyTorch</a>
        </def>
    <def title="Input Parameters">
        <deflist type="narrow">
            <def title="Images">
                RGB/A images
            </def>
            <def title="Scale Width">
                Determines the width of container
            </def>
            <def title="Scale Height">
                Determines the height of container
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
                    <li><control>Single</control> — Create only one container.</li>
                    <li><control>For Each</control> — Create container for each image in batch.</li>
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
