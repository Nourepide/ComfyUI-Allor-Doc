# Bokeh

<deflist type="narrow">
    <def title="Full Name">
        ImageEffectsLensBokeh
    </def>
    <def title="Description">
        Emulate a <a href="https://en.wikipedia.org/wiki/Bokeh">Bokeh</a> effect to images.
    </def>
        <def title="Backend">
            <a href="Modules.md" anchor="pytorch" summary="Image processing with pure Tensor without transformations.">PyTorch</a>
        </def>
    <def title="Input Parameters">
        <deflist type="narrow">
            <def title="Images">
                RGB/A images
            </def>
            <def title="Blades Shape">
                The number of blades at the lens
            </def>
            <def title="Blades Radius">
                Size of blades
            </def>
            <def title="Blades Rotation">
                Blades rotation in angles
            </def>
            <def title="Blur Size">
                Blur strength
            </def>
            <def title="Blur Type">
                <list>
                    <li><control>Bilateral</control> — Blur is set up to preserve sharp and bright edges.</li>
                    <li><control>Stack</control> — Blur with color correction.</li>
                    <li><control>None</control> — Without a blur.</li>
                </list>
            </def>
            <def title="Method">
                <list>
                    <li><control>Dilate</control> — A good choice for initially bright images. Creates a strong bokeh effect, but spoils the details of the image. I can recommend it only for the background.</li>
                    <li><control>Filter</control> — Very fast. A weak bokeh effect, I recommend it for dark images with bright rare details such as lamp lights or car headlights. Originally created under the impression of LensBlur in Adobe Photoshop and achieved about 80%~ compliance. I recommend setting blur_type as none since it blurs the image by itself.</li>
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
