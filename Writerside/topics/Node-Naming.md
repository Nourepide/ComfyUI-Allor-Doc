# Node Naming

At first glance, the node names in Allor may seem overly complex and long. However, don't rush to conclusions. The long
node names are not a coincidence, but a **thoughtful approach**.

All node names in Allor are created according to a **unified rule**. This makes them more understandable and
informative, allowing users to **quickly understand** what each node does, just by looking at its name.

The use of **descriptive names** is a good practice in programming, and it is widely used in many languages and
development environments.

### Example:

<procedure>
    <format color="Chartreuse">Image<format color="Crimson">Transform<format color="Gold">Resize<format color="SeaGreen">Relative</format></format></format></format>
    <list>
        <li><format color="Chartreuse">Image</format> — This is the <control>data type</control> that the node belongs to. <format color="Chartreuse">Image</format>, <format color="Chartreuse">Latent</format>, <format color="Chartreuse">Mask</format> and the fourth dimension of image <format color="Chartreuse">AlphaChannel</format> are currently available.</li>
        <li><format color="Crimson">Transform</format> — This is the <control>name of the module</control>. Nodes in this module usually perform transformation or conversion functions.</li>
        <li><format color="Gold">Resize</format> — This is the <control>functionality</control> of the node. The <format color="Gold">Resize</format> node is typically used to change the size of the image data.</li>
        <li><format color="SeaGreen">Relative</format> — This is a <control>postfix</control> that <control>further</control> describes the <control>functionality</control> of the node. It refers to the <control>precision</control> of the node’s operation, in contrast to the <format color="SeaGreen">Absolute</format> postfix. There is also an <format color="SeaGreen">Advanced</format> postfix, which implies more <control>extensive functionality</control>.</li>
    </list>
    <p>Simply by observing the node, you can discern its purpose: to <format color="Chartreuse">image data</format> <format color="Crimson">transform</format>, specifically adjusting <format color="Gold">tensor size</format> with <format color="SeaGreen">relative precision.</format></p>
</procedure>

## Exceptions

In some cases, the part with the <format color="Gold">node's name</format> can be omitted if the <format color="Crimson">module name</format> already sufficiently reflects its functionality. In such cases, the node's name in the documentation is indicated as **Default**.

This helps to simplify node names when additional details do not add significant information.
