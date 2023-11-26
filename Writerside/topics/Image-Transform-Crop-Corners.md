# Crop Corners

<deflist type="narrow">
    <def title="Full Name">
        ImageTransformCropCorners
    </def>
    <def title="Description">
        Rounds the corners of an images.
    </def>
        <def title="Backend">
            <a href="Modules.md" anchor="pillow" summary="A widely used Python library for image manipulation.">Pillow</a>
        </def>
    <def title="Input Parameters">
        <deflist type="narrow">
            <def title="Images">
                RGB/A images
            </def>
            <def title="Radius">
                The degree of rounding for the corners of the images.
            </def>
            <def title="Top Left Corner">
                Rounds the top left corner
            </def>
            <def title="Top Right Corner">
                Rounds the top right corner
            </def>
            <def title="Bottom Left Corner">
                Rounds the bottom left corner
            </def>
            <def title="Bottom Right Corner">
                Rounds the bottom right corner
            </def>
            <def title="SSAA">
                <control>S</control>uper-<control>S</control>ampling <control>A</control>nti-<control>A</control>liasing
                — is a technique where the image is temporarily upscale and modified at this higher resolution.
            </def>
            <def title="Method">
                <list>
                    <li><control>Lanczos</control> — A high-quality, computationally intensive resampling filter often used in professional-grade image processing software to resize images. It’s known for preserving high-frequency details.</li>
                    <li><control>Bicubic</control> — A commonly used method in image processing for resampling. It offers a good balance between image quality and computational efficiency. It’s widely adopted in much image processing software.</li>
                    <li><control>Hamming</control> — Predominantly used in computing, particularly in areas like error detection and correction. Its computation can get expensive when comparing a string against many strings.</li>
                    <li><control>Bilinear</control> — A fast and efficient algorithm that’s good for changing the size of an image, but it can cause some undesirable softening of details. It’s faster than bicubic and Lanczos, but generally provides lower quality results.</li>
                    <li><control>Box</control> — This method takes the target pixel of a box on the original image, and samples every pixel within the box, ensuring that all input pixels contribute to the output. While effective, this method can be difficult to optimize.</li>
                    <li><control>Nearest</control> — Also known as nearest-neighbor, this is the fastest and simplest interpolation method, often used when speed is more important than quality. It can result in a blocky image when upscaling.</li>
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
