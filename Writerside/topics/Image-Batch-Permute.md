# Permute

<deflist type="narrow">
    <def title="Full Name">
        ImageBatchPermute
    </def>
    <def title="Description">
        The ultimate way to work with batch of images. Allows you to rearrange, copy and remove images.
    </def>
        <def title="Backend">
            <a href="Modules.md" anchor="pytorch" summary="Image processing with pure Tensor without transformations.">PyTorch</a>
        </def>
    <def title="Input Parameters">
        <deflist type="narrow">
            <def title="Images">
                RGB/A images
            </def>
            <def title="Permute">
                <p>New order of images</p>
                <p>Wait for string input of <control>numbers</control> like &quot;1 3 2 4&quot;</p>
                <p><control>Numbers</control> can have any characters between them. &quot;1er!3,0002.4&quot; will be processed as [1, 3, 2, 4]</p>
                <p>Images can be <control>copied</control>. &quot;1 1 1 1&quot; return you 4 images with index 1</p>
                <p>And finally, the images can be <control>removed</control>. &quot;1 4&quot; will skip the image with index 2 and 3</p>
            </def>
            <def title="Start with zero">
                Order start with zero if true and with one if false
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
