# Fork

<deflist type="narrow">
    <def title="Full Name">
        ImageBatchFork
    </def>
    <def title="Description">
        Splits the batch in two.
    </def>
        <def title="Backend">
            <a href="Modules.md" anchor="pytorch" summary="Image processing with pure Tensor without transformations.">PyTorch</a>
        </def>
    <def title="Input Parameters">
        <deflist type="narrow">
            <def title="Images">
                RGB/A images
            </def>
            <def title="Priority">
                <list>
                    <li><control>First</control> — In case of an odd number, the center image will be sent to the first batch.</li>
                    <li><control>Second</control> — In case of an odd number, the center image will be sent to the second batch.</li>
                </list>
            </def>
        </deflist>
    </def>
    <def title="Output Parameters">
        <deflist type="narrow">
            <def title="Images">
                RGB/A images
            </def>
            <def title="Images">
                RGB/A images
            </def>
        </deflist>
    </def>
</deflist>
