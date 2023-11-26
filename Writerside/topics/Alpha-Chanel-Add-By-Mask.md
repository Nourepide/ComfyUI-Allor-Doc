# Add By Mask

<deflist type="narrow">
    <def title="Full Name">
        AlphaChannelAddByMask
    </def>
    <def title="Description">
        Getting alpha channels as mask and adding it to images.
    </def>
        <def title="Backend">
            <a href="Modules.md" anchor="pytorch" summary="Image processing with pure Tensor without transformations.">PyTorch</a>
        </def>
    <def title="Input Parameters">
        <deflist type="full">
            <def title="Images (Type: Image)">
                RGB images
            </def>
            <def title="Mask (Type: Mask)">
                Alpha Channel
            </def>
            <def title="Method (Type: Enum)">
                <list>
                    <li><control>Default</control> — Standard channel addition.</li>
                    <li><control>Invert</control> — The channel is changed to opposite values before being added.</li>
                </list>
            </def>
        </deflist>
    </def>
    <def title="Output Parameters">
        <deflist type="full">
            <def title="Images (Type: Image)">
                RGBA images
            </def>
        </deflist>
    </def>
</deflist>
