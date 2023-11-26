# As Mask

<deflist type="narrow">
    <def title="Full Name">
        AlphaChannelAsMask
    </def>
    <def title="Description">
        Copying alpha channels from images and return it.
    </def>
        <def title="Backend">
            <a href="Modules.md" anchor="pytorch" summary="Image processing with pure Tensor without transformations.">PyTorch</a>
        </def>
    <def title="Input Parameters">
        <deflist type="narrow">
            <def title="Images">
                RGBA images
            </def>
            <def title="Method">
                <list>
                    <li><control>Default</control> — Standard channel addition.</li>
                    <li><control>Invert</control> — The channel is changed to opposite values before being returned.</li>
                </list>
            </def>
        </deflist>
    </def>
    <def title="Output Parameters">
        <deflist type="narrow">
            <def title="Mask">
                Alpha Channel
            </def>
        </deflist>
    </def>
</deflist>
