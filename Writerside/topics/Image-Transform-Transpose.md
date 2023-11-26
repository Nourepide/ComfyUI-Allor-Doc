# Transpose

<deflist type="narrow">
    <def title="Full Name">
        ImageTransformTranspose
    </def>
    <def title="Description">
        Provides control over the orientation and location of images.
    </def>
        <def title="Backend">
            <a href="Modules.md" anchor="pillow" summary="A widely used Python library for image manipulation.">Pillow</a>
        </def>
    <def title="Input Parameters">
        <deflist type="narrow">
            <def title="Images">
                RGB/A images
            </def>
            <def title="Method">
                <list>
                    <li><control>Flip Horizontally</control> — Reflects the image horizontally.</li> 
                    <li><control>Flip Vertically</control> — Reflects the image vertically.</li> 
                    <li><control>Rotate 90</control> — Rotates the image 90 degrees clockwise.</li> 
                    <li><control>Rotate 180</control> — Rotates the image 180 degrees clockwise.</li> 
                    <li><control>Rotate 270</control> — Rotates the image 270 degrees clockwise.</li> 
                    <li><control>Transpose</control> — Reflects the image across the main diagonal (from top-left to bottom-right).</li> 
                    <li><control>Transverse</control> — Reflects the image across the secondary diagonal (from top-right to bottom-left).</li>
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
