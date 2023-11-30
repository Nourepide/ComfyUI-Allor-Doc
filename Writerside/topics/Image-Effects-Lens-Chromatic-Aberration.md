# Chromatic Aberration

<deflist type="narrow">
    <def title="Full Name">
        ImageEffectsLensChromaticAberration
    </def>
    <def title="Description">
        Apply a camera lens color shift to the images.
    </def>
        <def title="Backend">
            <a href="Modules.md" anchor="pytorch" summary="Image processing with pure Tensor without transformations.">PyTorch</a>
        </def>
    <def title="Input Parameters">
        <deflist type="narrow">
            <def title="Images">
                RGB/A images
            </def>
            <def title="Shift">
                Color shift in PX
            </def>
            <def title="Method">
                <list>
                    <li><control>Reflect</control> — The new space reflects the images around the edges.</li>
                    <li><control>Edge</control> — The new space is filled with pixels at the edges of the image.</li>
                    <li><control>Constant</control> — The new space is filled with emptiness.</li>
                </list>
            </def>
            <def title="Shift Type">
                Type of chromatic aberration
            </def>
            <def title="Mixing Type">
                Type of method for shifting colors
            </def>
            <def title="Transpose">
                <list>
                    <li><control>None</control> — Without a change of direction.</li>
                    <li><control>Rotate</control> — Alternative direction.</li>
                    <li><control>Reflect</control> — In both directions at the same time.</li>
                </list>
            </def>
           <def title="Colors">
                <list>
                    <li><control>rb</control> — Red and Blue color channels.</li>
                    <li><control>rg</control> — Red and Green color channels.</li>
                    <li><control>gb</control> — Green and Blue color channels.</li>
                </list>
            </def>
            <def title="Lens Curvy">
                The value of the curve during the propagation of the effect, where 1.0 is linear. 
                Not working with shift_type 4.
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
