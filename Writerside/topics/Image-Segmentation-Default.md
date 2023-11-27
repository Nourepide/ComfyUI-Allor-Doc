# Default

<deflist type="narrow">
    <def title="Full Name">
        ImageSegmentation
    </def>
    <def title="Description">
        Removes background from images.
    </def>
        <def title="Backend">
            <a href="Modules.md" anchor="rembg" summary="A specialized library for removing image backgrounds.">Rembg</a>
        </def>
    <def title="Input Parameters">
        <deflist type="narrow">
            <def title="Images">
                RGB/A images
            </def>
            <def title="Model">
                <list>
                    <li><control>u2net</control> — <a href="https://github.com/xuebinqin/U-2-Net">GitHub</a>.</li>
                    <li><control>u2netp</control> — <a href="https://github.com/xuebinqin/U-2-Net">GitHub</a>.</li>
                    <li><control>u2net_human_seg</control> — <a href="https://github.com/xuebinqin/U-2-Net">GitHub</a>.</li>
                    <li><control>u2net_cloth_seg</control> — <a href="https://github.com/levindabhi/cloth-segmentation">GitHub</a>.</li>
                    <li><control>siluetta</control> — <a href="https://github.com/xuebinqin/U-2-Net/issues/295">GitHub</a>.</li>
                    <li><control>isnet</control> — <a href="https://github.com/xuebinqin/DIS">GitHub</a>.</li>
                    <li><control>isnetis</control> — <a href="https://github.com/SkyTNT/anime-segmentation">GitHub</a>.</li>
                    <li><control>modnet-p</control> — <a href="https://github.com/ZHKKKe/MODNet">GitHub</a>.</li>
                    <li><control>modnet-w</control> — <a href="https://github.com/ZHKKKe/MODNet">GitHub</a>.</li>
                </list>
            </def>
            <def title="Alpha Matting">
                Alpha matting is a post-processing step that can be used to improve the quality of the output
            </def>
            <def title="Alpha Matting Foreground Threshold">
                Trimap foreground threshold
            </def>
            <def title="Alpha Matting Background Threshold">
                Trimap background threshold
            </def>
            <def title="Alpha Matting Erode Size">
                How far will the transparency spread from the original mask
            </def>
            <def title="Post-Process Mask">
                Post-processing mask, makes it rougher
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
