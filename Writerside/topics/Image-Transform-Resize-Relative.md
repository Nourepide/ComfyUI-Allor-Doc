# Resize Relative

<deflist type="narrow">
    <def title="Full Name">
        ImageTransformResizeRelative
    </def>
    <def title="Description">
        Changes images size by scale factor.
    </def>
        <def title="Backend">
            <a href="Modules.md" anchor="pytorch" summary="Image processing with pure Tensor without transformations.">PyTorch</a>
        </def>
    <def title="Input Parameters">
        <deflist type="narrow">
            <def title="Images">
                RGB/A images
            </def>
            <def title="Width">
                New width in a scale factor where 1.0 is original size
            </def>
            <def title="Height">
                New height in a scale factor where 1.0 is original size
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
            <def title="Images">
                RGB/A images
            </def>
        </deflist>
    </def>
</deflist>

