# Zoom Burst

<deflist type="narrow">
    <def title="Full Name">
        ImageEffectsLensZoomBurst
    </def>
    <def title="Description">
        Emulate a <a href="https://en.wikipedia.org/wiki/Zoom_burst">Zoom Burst</a> effect to images.
    </def>
        <def title="Backend">
            <a href="Modules.md" anchor="pytorch" summary="Image processing with pure Tensor without transformations.">PyTorch</a>
        </def>
    <def title="Input Parameters">
        <deflist type="narrow">
            <def title="Images">
                RGB/A images
            </def>
            <def title="Scale">
                How far the zoom will aim. Where <control>2.0</control> is <control>x2</control> from image size
            </def>
            <def title="Samples">
                How many intermediate frames will be created
            </def>
            <def title="Position X">
                Relative vertical image position
            </def>
            <def title="Position Y">
                Relative horizontal image position
            </def>
            <def title="Rotation">
                Rotation in angle
            </def>
            <def title="Method">
                <list>
                    <li><control>Circle</control> — Zoom will spread out in the form of a circle, and do not take into account the boundaries of the images.</li>
                    <li><control>Point</control> — Zoom will spread out from point to boundaries of the images.</li>
                </list>
            </def>
            <def title="Stabilization">
                If set to true, the images will retain their size
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
