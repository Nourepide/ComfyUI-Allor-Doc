# Rectangle By Container

<deflist type="narrow">
    <def title="Full Name">
        ImageDrawRectangleByContainer
    </def>
    <def title="Description">
        Draws a rectangle.
    </def>
        <def title="Backend">
            <a href="Modules.md" anchor="pillow" summary="A widely used Python library for image manipulation.">Pillow</a>
        </def>
    <def title="Input Parameters">
        <deflist type="narrow">
            <def title="Container">
                Container size
            </def>
            <def title="Width">
                Width of container
            </def>
            <def title="Height">
                Height of container
            </def>
            <def title="Start X">
                Start vertical point to define the bounding box in percentage of image container
            </def>
            <def title="Start Y">
                Start horizontal point to define the bounding box in percentage of image container
            </def>
            <def title="End X">
                End vertical point to define the bounding box in percentage of image container
            </def>
            <def title="End Y">
                End horizontal point to define the bounding box in percentage of image container
            </def>
            <def title="Outline Size">
                Outline size
            </def>
            <def title="Outline Red">
                Red channel of outline color
            </def>
            <def title="Outline Green">
                Green channel of outline color
            </def>
            <def title="Outline Blue">
                Blue channel of outline color
            </def>
            <def title="Outline Alpha">
                Alpha channel of outline color
            </def>
            <def title="Fill Red">
                Red channel of color
            </def>
            <def title="Fill Green">
                Green channel of color
            </def>
            <def title="Fill Blue">
                Blue channel of color
            </def>
            <def title="Fill Alpha">
                Alpha channel of color
            </def>
            <def title="SSAA">
                <control>S</control>uper-<control>S</control>ampling <control>A</control>nti-<control>A</control>liasing
                — is a technique where the image is temporarily upscale and modified at this higher resolution.
            </def>
            <def title="Method">
                <list>
                    <li><control>Lanczos</control> — A high-quality, computationally intensive resampling filter often used in professional-grade image processing software to resize images. It’s known for preserving high-frequency details.</li>
                    <li><control>Bicubic</control> — A commonly used method in image processing for resampling. It offers a good balance between image quality and computational efficiency. It’s widely adopted in much image processing software.</li>
                    <li><control>Hamming</control> — While not typically used for image resizing, the Hamming algorithm is ubiquitous in computing, particularly in areas like error detection and correction. Its computation can get expensive when comparing a string against many strings.</li>
                    <li><control>Bilinear</control> — A fast and efficient algorithm that’s good for changing the size of an image, but it can cause some undesirable softening of details. It’s faster than bicubic and Lanczos, but generally provides lower quality results.</li>
                    <li><control>Box</control> — This method takes the target pixel of a box on the original image, and samples every pixel within the box, ensuring that all input pixels contribute to the output. While effective, this method can be difficult to optimize.</li>
                    <li><control>Nearest</control> — Also known as nearest-neighbor, this is the fastest and simplest interpolation method, often used when speed is more important than quality. It can result in a blocky image when upscaling.</li>
                </list>
            </def>
        </deflist>
    </def>
    <def title="Output Parameters">
        <deflist type="narrow">
            <def title="Image">
                RGBA image
            </def>
        </deflist>
    </def>
</deflist>
